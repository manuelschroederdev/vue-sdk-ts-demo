<template>
  <div v-editable="blok" class="flex py-8 mb-6">
    <div v-for="blok in blok.columns" :key="blok._uid" class="flex-auto px-6">
      <StoryblokComponent :blok="blok" />
    </div>
  </div>
</template>

<script setup lang="ts">
import type { SbBlokData } from '@storyblok/vue'

export interface SbComponentProps {
  blok: SbBlokData
}
defineProps<SbComponentProps>()
</script>
