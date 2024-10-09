<template>
  <UModal title="Modal with description" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit.">
    <UButton label="Open" />

    <template #body>
      <USelectMenu v-model="value" :items="items" />

    </template>
  </UModal>
</template>
<script setup lang="ts">
const items = ref(['Backlog', 'Todo', 'In Progress', 'Done'])
const value = ref('Backlog')
</script>