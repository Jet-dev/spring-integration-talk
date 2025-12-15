<template>
  <div class="slidev-layout letter-background">
    <div class="glass-panel p-4 rounded-xl absolute top-6 right-6 bottom-6 left-6
flex ">
      <div class="left flex-1">
        <slot name="left" />
      </div>
      <div class="right flex-1">
        <slot name="right" />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
</script>
