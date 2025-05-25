<script setup lang="ts">
import { ref } from "vue"
import { Popover } from "@ark-ui/vue/popover"

const open = ref(false)
</script>

<template>
  <Popover.Root v-model:open="open">
    <Popover.Trigger
      class="flex items-center gap-2 cursor-pointer bg-gray-200 p-2"
    >
      Click Me
      <Popover.Indicator>{{ open ? "v" : ">" }}</Popover.Indicator>
    </Popover.Trigger>
    <Popover.Positioner>
      <Popover.Content>
        <Popover.Title>Title1</Popover.Title>
        <Popover.Description>Description</Popover.Description>
      </Popover.Content>
      <Popover.Content>
        <Popover.Title>Title2</Popover.Title>
        <Popover.Description>Description</Popover.Description>
      </Popover.Content>
      <Popover.Content>
        <Popover.Title>Title3</Popover.Title>
        <Popover.Description>Description</Popover.Description>
      </Popover.Content>
    </Popover.Positioner>
  </Popover.Root>
</template>
