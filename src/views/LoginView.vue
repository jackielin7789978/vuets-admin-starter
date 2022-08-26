<script lang="ts" setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <div>
    <h1 class="title">Vuets Admin</h1>
    <p class="text-center mb-4 text-gray-400">
      place your login component here
    </p>
    <router-link to="/">
      <a-button type="primary" size="large" class="w-full">Login</a-button>
    </router-link>
  </div>
</template>

<style lang="scss" scoped>
.title {
  font-size: 48px;
  font-weight: 700;
  background: linear-gradient(to right, #42b883 0%, #3f9eef 100%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  user-select: none;
}
</style>
