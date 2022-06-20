<template>
  <div v-editable="blok" class="py-2">
    <h1 class="text-lg">{{ blok.name }}</h1>
  </div>
</template>

<script setup lang="ts">
import type { SbBlokData } from '@storyblok/vue'

export interface SbComponentProps {
  blok: SbBlokData
}
defineProps<SbComponentProps>()
</script>
