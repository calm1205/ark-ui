<script setup lang="ts">
import { Slider } from "@ark-ui/vue/slider"
</script>

<template>
  <Slider.Root>
    <Slider.Label>Label</Slider.Label>
    <Slider.ValueText />
    <Slider.Control>
      <Slider.Track>
        <Slider.Range />
      </Slider.Track>
      <Slider.Thumb :index="0">
        <Slider.HiddenInput />
      </Slider.Thumb>
    </Slider.Control>
  </Slider.Root>
</template>

<style scoped>
/* Targets the <Slider.Root /> */
[data-scope="slider"][data-part="root"] {
  display: flex;
  flex-direction: column;
}
</style>
