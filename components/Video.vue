<template>
  <div class="rounded overflow-hidden h-95 w-fit mx-auto" style="margin-top: -25px">
    <video ref="videoElement" class="w-full h-full" muted />
  </div>
  <div v-if="caption" class="text-center mt-4">
    {{ caption }}
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { onSlideEnter } from '@slidev/client'

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

const videoElement = ref(null);

onSlideEnter(() => {
  if (videoElement.value) {
    videoElement.value.src = props.src
    videoElement.value.currentTime = 0
    videoElement.value.play()
  }
})
</script>
