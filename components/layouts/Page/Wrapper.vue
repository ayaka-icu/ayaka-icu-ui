<script setup lang="ts">
import { defineProps } from 'vue'
const props = defineProps({
  py: {
    type: Boolean,
    default: true
  }
})
</script>
<template>
  <div class="flex-1 max-w-screen-2xl w-full px-4 mx-auto" :class="{ 'py-4': py}">
    <slot />
  </div>
</template>
