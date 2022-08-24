<template>
  <TheWelcome />
  <RouterView class="mt-8" />
</template>

<style>
#app {
  width: 80%;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  row-gap: 1rem;
}
</style>
