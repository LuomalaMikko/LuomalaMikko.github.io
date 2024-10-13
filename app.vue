<template>
    <NuxtLayout :name="layout">
      <NuxtPage />
    </NuxtLayout>
  </template>
  
  <script setup lang="ts">
  //Error handling starts
  import { showError } from '#imports'
  const route = useRoute()
  if ('setup' in route.query) {
  throw new Error('error in setup')
  }
  if ('mounted' in route.query) {
  onMounted(() => {
    throw new Error('error in mounted')
  })
  }
  function triggerError() {
  throw new Error('manually triggered error')
  }
  // Error handling ends
  
  const layout = "default";
  
  </script>
  