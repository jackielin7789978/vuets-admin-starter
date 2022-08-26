<script setup lang="ts">
import TheHeader from './components/TheHeader.vue'
import TheSider from './components/TheSider.vue'
</script>

<template>
  <a-layout>
    <TheSider />
    <a-layout>
      <TheHeader />
      <a-layout-content class="content">
        <slot></slot>
      </a-layout-content>
    </a-layout>
  </a-layout>
</template>

<style lang="scss" scoped>
.content {
  padding: 0.5rem 1rem;
}
</style>
