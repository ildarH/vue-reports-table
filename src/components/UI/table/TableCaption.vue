<script setup lang="ts">
import type { HTMLAttributes } from 'vue'
import { cn } from '@/lib/utils'

const props = defineProps<{
  class?: HTMLAttributes['class']
}>()
</script>

<template>
  <caption :class="cn('mt-1 text-sm text-muted-foreground', props.class)" id="tableCaption">
    <slot />
  </caption>
</template>
