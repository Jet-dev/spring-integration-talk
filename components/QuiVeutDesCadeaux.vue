<template>
  <div class="relative w-full h-full">
    <div class="relative z-10 flex flex-col items-center justify-center h-full text-center text-white">
      <div class="gift-box animate-gift-reveal">
        <span class="text-6xl">{{ giftIcon }}</span>
      </div>

      <h1 class="text-4xl font-extrabold tracking-tight drop-shadow-lg leading-tight animate-fade-in-up mt-4">
        {{ title }}
      </h1>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps({
  title: {
    type: String,
    required: true,
  },
  giftIcon: {
    type: String,
    default: '🎁',
  }
});
</script>

<style scoped>

@keyframes gift-reveal {
  0% { transform: scale(0) rotate(-180deg); opacity: 0; }
  50% { transform: scale(1.5) rotate(10deg); opacity: 1; }
  75% { transform: scale(0.9) rotate(-5deg); }
  100% { transform: scale(1) rotate(0deg); }
}
.animate-gift-reveal {
  animation: gift-reveal 1.5s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards;
}

@keyframes fade-in-up {
  from { opacity: 0; transform: translateY(40px); }
  to { opacity: 1; transform: translateY(0); }
}
.animate-fade-in-up {
  animation: fade-in-up 1s ease-out forwards;
  animation-delay: 0.3s;
  opacity: 0;
}
</style>
