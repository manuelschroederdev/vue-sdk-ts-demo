<template>
  <div v-editable="blok" class="px-6">
    <StoryblokComponent
      v-for="blok in blok.body"
      :blok="blok"
      :key="blok._uid"
    />
  </div>
</template>

<script setup lang="ts">
import type { SbBlokData } from '@storyblok/vue'

export interface SbComponentProps {
  blok: SbBlokData
}
defineProps<SbComponentProps>()
</script>
