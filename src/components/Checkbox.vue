<script setup lang="ts">
import { Checkbox } from "@ark-ui/vue/checkbox"

const props = defineProps<{
  label: string
}>()
</script>

<template>
  <Checkbox.Root class="flex">
    <Checkbox.Label>{{ props.label }}</Checkbox.Label>
    <Checkbox.Control>
      <Checkbox.Indicator> ✓ </Checkbox.Indicator>
    </Checkbox.Control>
    <Checkbox.HiddenInput />
  </Checkbox.Root>
</template>

<style scoped>
[data-part="root"] {
  align-items: center;
  gap: 5px;
  cursor: pointer;
}
[data-part="control"] {
  min-width: 15px;
  height: 15px;
  border: 1px solid black;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
