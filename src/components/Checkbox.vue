<script setup lang="ts">
import { Checkbox } from "@ark-ui/vue/checkbox"

const props = defineProps<{
  label: string
}>()
</script>

<template>
  <Checkbox.Root class="flex items-center gap-2 cursor-pointer">
    <Checkbox.Label>{{ props.label }}</Checkbox.Label>
    <Checkbox.Control
      class="flex items-center justify-center min-w-[15px] h-[15px] border border-black"
    >
      <Checkbox.Indicator> ✓ </Checkbox.Indicator>
    </Checkbox.Control>
    <Checkbox.HiddenInput />
  </Checkbox.Root>
</template>
