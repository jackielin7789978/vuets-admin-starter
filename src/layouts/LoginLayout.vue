<template>
  <div class="login-wrapper">
    <div class="login-component">
      <slot></slot>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.login-wrapper {
  position: relative;
  height: 100%;
  background-color: #f5f5f5;
}
.login-component {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
}
</style>
