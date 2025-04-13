<template>
    <header class="p-4 md:p-6">
        <div class="container mx-auto">
            <nav aria-label="Main Navigation" class="flex items-center justify-between">            
                <div class="flex items-center justify-between w-full">
                    <NuxtLink to="/" class="z-50 w-auto" @click="isOpen = false">
                        <svg id="Layer_1" class="w-2/4 md:h-10 md:w-full main-logo" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" fill="#fff" viewBox="0 0 354.29 56.35"><title>temp-log</title><path d="M0,19.36,37.58,0V5.59L5.91,21.46v.17L37.58,37.5v5.59L0,23.73Z"/><path d="M47.49,3.19a54.37,54.37,0,0,1,10-.84c5.58,0,9.18,1,11.7,3.3a10.07,10.07,0,0,1,3.18,7.68,10.62,10.62,0,0,1-7.62,10.32v.18c3.12,1.08,5,4,5.94,8.16C72,37.63,73,41.53,73.83,43.09h-5.4c-.66-1.14-1.56-4.62-2.7-9.66-1.2-5.58-3.36-7.68-8.1-7.86H52.71V43.09H47.49Zm5.22,18.42h5.34c5.58,0,9.12-3.06,9.12-7.68,0-5.22-3.78-7.5-9.3-7.56a21.48,21.48,0,0,0-5.16.48Z"/><path d="M86.07,5.89a3.27,3.27,0,0,1-6.54,0,3.22,3.22,0,0,1,3.3-3.3A3.13,3.13,0,0,1,86.07,5.89Zm-5.88,37.2v-29h5.28v29Z"/><path d="M114.93,42a19.45,19.45,0,0,1-8.34,1.68c-8.76,0-14.46-5.94-14.46-14.82s6.12-15.42,15.6-15.42a17.65,17.65,0,0,1,7.32,1.5L113.85,19a12.24,12.24,0,0,0-6.12-1.38c-6.66,0-10.26,4.92-10.26,11,0,6.72,4.32,10.86,10.08,10.86A15,15,0,0,0,114,38.05Z"/><path d="M121.11.49h5.28V18.61h.12a9.8,9.8,0,0,1,3.78-3.72,10.87,10.87,0,0,1,5.4-1.5c3.9,0,10.14,2.4,10.14,12.42V43.09h-5.28V26.41c0-4.68-1.74-8.64-6.72-8.64a7.59,7.59,0,0,0-7.08,5.28,6.39,6.39,0,0,0-.36,2.52V43.09h-5.28Z"/><path d="M188.67,25.33c-.3-5.64-.66-12.42-.6-17.46h-.18c-1.38,4.74-3.06,9.78-5.1,15.36l-7.14,19.62h-4l-6.54-19.26c-1.92-5.7-3.54-10.92-4.68-15.72h-.12c-.12,5-.42,11.82-.78,17.88l-1.08,17.34h-5l2.82-40.44H163l6.9,19.56c1.68,5,3.06,9.42,4.08,13.62h.18c1-4.08,2.46-8.52,4.26-13.62l7.2-19.56h6.66l2.52,40.44h-5.1Z"/><path d="M206,29.53c.12,7.14,4.68,10.08,10,10.08a19.09,19.09,0,0,0,8-1.5l.9,3.78a23.52,23.52,0,0,1-9.66,1.8c-8.94,0-14.28-5.88-14.28-14.64s5.16-15.66,13.62-15.66c9.48,0,12,8.34,12,13.68a19.91,19.91,0,0,1-.18,2.46Zm15.48-3.78c.06-3.36-1.38-8.58-7.32-8.58-5.34,0-7.68,4.92-8.1,8.58Z"/><path d="M233.07,23.11c0-3.42-.06-6.36-.24-9.06h4.62l.18,5.7h.24c1.32-3.9,4.5-6.36,8-6.36a5.71,5.71,0,0,1,1.5.18v5a7.93,7.93,0,0,0-1.8-.18c-3.72,0-6.36,2.82-7.08,6.78a14.86,14.86,0,0,0-.24,2.46V43.09h-5.22Z"/><path d="M256.11,14.05l6.36,17.16c.66,1.92,1.38,4.2,1.86,5.94h.12c.54-1.74,1.14-4,1.86-6.06l5.76-17h5.58l-7.92,20.7c-3.78,10-6.36,15.06-10,18.18a14.31,14.31,0,0,1-6.48,3.42L252,51.91a14,14,0,0,0,4.62-2.58A16,16,0,0,0,261,43.45a3.79,3.79,0,0,0,.42-1.26,4.6,4.6,0,0,0-.36-1.38L250.35,14.05Z"/><path d="M290.73,45.49,307.46,2h4.08l-16.79,43.5Z"/><path d="M354.29,23.81,316.71,43.09V37.5l31.91-15.87v-.17L316.71,5.59V0l37.58,19.28Z"/></svg>
                    </NuxtLink>
                    <button style="" class="block md:hidden text-3xl" :aria-expanded="isOpen" @click="isOpen = true">
                    <Icon name="ph:list-bold"/>
                    </button>              
                </div>
                <div :class="isOpen ? 'translate-x-0' : 'translate-x-full'" class="md:hidden fixed inset-0 z-40 flex flex-col items-end bg-neutral-900 pr-4 pt-6 transition-transform duration-300 ease-in-out will-change-transform">
                    <button style="" class="text-3xl" :aria-expanded="isOpen" @click="isOpen = false">
                    <Icon name="ph:x-bold"/>                    </button> 
                    <ul class="grid justify-items-end gap-6">
                        <li v-for="link in settings?.data.navigation" :key="link.key">
                            <PrismicLink :field="link" :class="link.variant" @click="isOpen = false"/>
                        </li>
                    </ul>
                </div>
                <ul class="hidden md:flex gap-6">
                    <li v-for="link in settings?.data.navigation" :key="link.key">
                        <PrismicLink :field="link" :class="link.variant" />
                    </li>
                </ul>          
            </nav>
        </div>
    </header>
</template>

<script lang="ts" setup>
import type { Content } from "@prismicio/client";

const isOpen = ref(false);
defineProps<{
    settings?: Content.SettingsDocument
}>()
</script>

<style>
.main-logo{
    filter: drop-shadow(0px 1px 9px lime);
    display: flex;
    align-self: center;
}
</style>