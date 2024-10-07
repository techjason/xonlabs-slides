<template>
    <div class="flappy-bird-game">
        <canvas ref="gameCanvas" width="400" height="400"></canvas>

        <div class="score">{{ score }}</div>
    </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const gameCanvas = ref(null);
const gameStarted = ref(false);
const score = ref(0);

let bird, pipes, ctx, animationFrameId;

const startGame = () => {
    gameStarted.value = true;
    initGame();
};

const initGame = () => {
    const canvas = gameCanvas.value;
    ctx = canvas.getContext("2d");

    bird = {
        x: 50,
        y: 200,
        velocity: 0,
        gravity: 0.25, // Reduced from 0.5
        jump: -6, // Changed from -10 to make it less strong
    };

    pipes = [];
    score.value = 0;

    gameLoop();
};

const gameLoop = () => {
    update();
    draw();
    animationFrameId = requestAnimationFrame(gameLoop);
};

const update = () => {
    bird.velocity += bird.gravity;
    bird.y += bird.velocity;

    if (bird.y + 20 > 400) {
        endGame();
    }

    // Increase the distance between pipes even more
    if (pipes.length === 0 || pipes[pipes.length - 1].x < 100) {
        pipes.push({
            x: 400,
            topHeight: Math.random() * 150 + 50,
        });
    }

    pipes.forEach((pipe) => {
        // Pipe movement speed remains the same
        pipe.x -= 1.5;

        if (pipe.x + 50 < 0) {
            pipes.shift();
            score.value++;
        }

        if (
            bird.x + 20 > pipe.x &&
            bird.x < pipe.x + 50 &&
            (bird.y < pipe.topHeight || bird.y + 20 > pipe.topHeight + 150)
        ) {
            endGame();
        }
    });
};

const draw = () => {
    ctx.clearRect(0, 0, 400, 400);

    ctx.fillStyle = "yellow";
    ctx.fillRect(bird.x, bird.y, 20, 20);

    pipes.forEach((pipe) => {
        ctx.fillStyle = "green";
        ctx.fillRect(pipe.x, 0, 50, pipe.topHeight);
        ctx.fillRect(
            pipe.x,
            pipe.topHeight + 150,
            50,
            400 - pipe.topHeight - 150
        );
    });
};

const endGame = () => {
    cancelAnimationFrame(animationFrameId);
    gameStarted.value = false;
    // Reset game state
    bird = null;
    pipes = [];
    // Clear the canvas
    ctx.clearRect(0, 0, 400, 400);
};

const jump = () => {
    if (gameStarted.value) {
        bird.velocity = bird.jump;
    } else {
        startGame();
    }
};

const handleKeyPress = (e) => {
    if (e.key.toLowerCase() === "j") {
        jump();
    }
};

onMounted(() => {
    window.addEventListener("keydown", handleKeyPress);
});

onUnmounted(() => {
    window.removeEventListener("keydown", handleKeyPress);
    cancelAnimationFrame(animationFrameId);
});
</script>

<style scoped>
.flappy-bird-game {
    position: relative;
    width: 400px;
    height: 400px;
    margin: 0 auto;
    cursor: pointer; /* Add this line to show a pointer cursor on hover */
}

.start-screen {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.score {
    position: absolute;
    top: 10px;
    right: 10px;
    font-size: 20px;
    font-weight: bold;
}

.instructions {
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 16px;
    font-weight: bold;
}
</style>
