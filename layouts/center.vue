<script setup lang="ts">
  import CoverCornerBadge from "slidev-theme-lcpu/components/CoverCornerBadge.vue";
</script>

<template>
  <div class="slidev-layout center h-full grid place-content-center">
    <div class="my-auto">
      <slot />
    </div>
    <CoverCornerBadge />
  </div>
</template>
