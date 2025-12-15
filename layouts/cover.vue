<template>
  <div class="slidev-layout cover">
    <div class="my-auto w-full text-center">
      <div class="glass-panel p-10 rounded-xl inline-block">
        <slot />
      </div>
    </div>
  </div>
</template>

<style scoped>
.glass-panel {
  background: rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(5px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
}

:deep(h1) {
  font-size: 3.5rem;
  font-weight: 800;
  margin-bottom: 1rem;
  background: linear-gradient(45deg, #FF772C, #FF772C); /* Gradient text */
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-shadow: none;
}

:deep(h3) {
  font-size: 1.8rem;
  color: #a0aec0;
  margin-bottom: 2rem;
}
</style>