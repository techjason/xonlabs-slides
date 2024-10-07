<template>
    <div
        :class="[
            'absolute inset-0 mx-auto aspect-[1/1] w-full max-w-[600px] z-[-1]',
            className,
        ]"
    >
        <canvas
            ref="canvasRef"
            :class="[
                'size-full opacity-0 transition-opacity duration-500 [contain:layout_paint_size]',
            ]"
            @pointerdown="onPointerDown"
            @pointerup="onPointerUp"
            @pointerout="onPointerUp"
            @mousemove="onMouseMove"
            @touchmove="onTouchMove"
        />
    </div>
</template>

<script setup lang="ts">
import { ref, onMounted, onUnmounted, watch } from "vue";
import createGlobe, { COBEOptions } from "cobe";

const props = defineProps({
    className: {
        type: String,
        default: "",
    },
    config: {
        type: Object as () => COBEOptions,
        default: () => ({
            width: 800,
            height: 800,
            onRender: () => {},
            devicePixelRatio: 2,
            phi: 0,
            theta: 0.3,
            dark: 0,
            diffuse: 0.4,
            mapSamples: 16000,
            mapBrightness: 1.2,
            baseColor: [1, 1, 1],
            markerColor: [251 / 255, 100 / 255, 21 / 255],
            glowColor: [1, 1, 1],
            markers: [
                { location: [14.5995, 120.9842], size: 0.03 },
                { location: [19.076, 72.8777], size: 0.1 },
                { location: [23.8103, 90.4125], size: 0.05 },
                { location: [30.0444, 31.2357], size: 0.07 },
                { location: [39.9042, 116.4074], size: 0.08 },
                { location: [-23.5505, -46.6333], size: 0.1 },
                { location: [19.4326, -99.1332], size: 0.1 },
                { location: [40.7128, -74.006], size: 0.1 },
                { location: [34.6937, 135.5022], size: 0.05 },
                { location: [41.0082, 28.9784], size: 0.06 },
            ],
        }),
    },
});

const canvasRef = ref<HTMLCanvasElement | null>(null);
const pointerInteracting = ref<number | null>(null);
const pointerInteractionMovement = ref(0);
const r = ref(0);
let phi = 0;
let width = 0;
let globeInstance: any = null;

const updatePointerInteraction = (value: number | null) => {
    pointerInteracting.value = value;
    if (canvasRef.value) {
        canvasRef.value.style.cursor = value !== null ? "grabbing" : "grab";
    }
};

const updateMovement = (clientX: number) => {
    if (pointerInteracting.value !== null) {
        const delta = clientX - pointerInteracting.value;
        pointerInteractionMovement.value = delta;
        r.value = delta / 200;
    }
};

const onRender = (state: Record<string, any>) => {
    if (pointerInteracting.value === null) phi += 0.005;
    state.phi = phi + r.value;
    state.width = width * 2;
    state.height = width * 2;
};

const onResize = () => {
    if (canvasRef.value) {
        width = canvasRef.value.offsetWidth;
    }
};

const onPointerDown = (e: PointerEvent) => {
    updatePointerInteraction(e.clientX - pointerInteractionMovement.value);
};

const onPointerUp = () => {
    updatePointerInteraction(null);
};

const onMouseMove = (e: MouseEvent) => {
    updateMovement(e.clientX);
};

const onTouchMove = (e: TouchEvent) => {
    if (e.touches[0]) {
        updateMovement(e.touches[0].clientX);
    }
};

onMounted(() => {
    window.addEventListener("resize", onResize);
    onResize();

    if (canvasRef.value) {
        globeInstance = createGlobe(canvasRef.value, {
            ...props.config,
            width: width * 2,
            height: width * 2,
            onRender,
        });

        setTimeout(() => {
            if (canvasRef.value) {
                canvasRef.value.style.opacity = "1";
            }
        });
    }
});

onUnmounted(() => {
    window.removeEventListener("resize", onResize);
    if (globeInstance) {
        globeInstance.destroy();
    }
});

watch(
    () => props.config,
    (newConfig) => {
        if (globeInstance) {
            globeInstance.destroy();
            globeInstance = createGlobe(canvasRef.value!, {
                ...newConfig,
                width: width * 2,
                height: width * 2,
                onRender,
            });
        }
    },
    { deep: true }
);
</script>
