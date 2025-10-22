<template>
  <div class="rounded overflow-hidden h-95 w-fit mx-auto" style="margin-top: -25px">
    <img class="w-full h-full" :src="src" />
  </div>
  <div v-if="caption" class="text-center mt-4">
    {{ caption }}
  </div>
</template>

<script setup>
const props = defineProps({
  src: {
    type: String,
    required: true
  },
  caption: {
    type: String,
    default: ''
  }
})
</script>
