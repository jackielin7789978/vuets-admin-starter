<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>
<template>
  <h1 class="cool-title">
    Vue 3, TypeScript, Ant Design Vue & WindiCSS ready for <span>YOU</span>
  </h1>
  <nav>
    <a-button type="link"><RouterLink to="/">Home</RouterLink></a-button>
    <a-button type="link"><RouterLink to="/about">About</RouterLink></a-button>
  </nav>
</template>

<style lang="scss" scoped>
.cool-title {
  font-size: 48px;
  font-weight: 700;
  background: linear-gradient(to right, #42b883 0%, #3f9eef 100%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>
