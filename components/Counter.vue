<template>
    <div class="counter-container">
        <div class="count-display">{{ count }}</div>
        <button
            @click="increment"
            class="increment-button"
            aria-label="Increment"
        >
            <svg
                xmlns="http://www.w3.org/2000/svg"
                width="20"
                height="20"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
            >
                <line x1="12" y1="5" x2="12" y2="19"></line>
                <line x1="5" y1="12" x2="19" y2="12"></line>
            </svg>
        </button>
    </div>
</template>

<script setup>
import { ref } from "vue";

const count = ref(0);

function increment() {
    count.value++;
}
</script>

<style scoped>
.counter-container {
    position: absolute;
    bottom: 20px;
    left: 20px;
    display: flex;
    align-items: center;
    background-color: var(--geist-background);
    border: 1px solid var(--accents-2);
    border-radius: 6px;
    overflow: hidden;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.count-display {
    padding: 8px 12px;
    font-size: 16px;
    font-weight: 500;
    color: var(--geist-foreground);
    border-right: 1px solid var(--accents-2);
}

.increment-button {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 36px;
    height: 36px;
    background-color: transparent;
    border: none;
    cursor: pointer;
    transition: background-color 0.2s ease;
}

.increment-button:hover {
    background-color: var(--accents-1);
}

.increment-button svg {
    color: var(--geist-foreground);
}
</style>
