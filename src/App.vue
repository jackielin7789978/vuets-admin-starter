<script setup lang="ts">
import DefaultLayout from './layouts/DefaultLayout.vue'
import { useRoute } from 'vue-router'

const route = useRoute()
</script>

<template>
  <component :is="route.meta.layout ?? DefaultLayout" id="real-app">
    <RouterView />
  </component>
</template>

<style>
#app {
  position: relative;
  height: 100%;
}
#real-app {
  min-height: 100%;
}
</style>
