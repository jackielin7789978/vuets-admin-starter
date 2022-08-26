<script setup lang="ts">
import { ref } from 'vue'
import { RouterLink } from 'vue-router'
import {
  ControlOutlined,
  ApartmentOutlined,
  DashboardOutlined,
  TeamOutlined,
  DatabaseOutlined,
  LoginOutlined
} from '@ant-design/icons-vue'
const selectedKeys = ref<string[]>(['1'])
</script>
<template>
  <a-layout-sider collapsible breakpoint="lg" width="240">
    <div class="logo"></div>
    <a-menu v-model:selectedKeys="selectedKeys" mode="inline" theme="dark">
      <a-menu-item key="1">
        <template #icon> <dashboard-outlined /></template>
        <span>Dashboard</span>
      </a-menu-item>
      <a-menu-item key="2">
        <template #icon> <control-outlined /></template>
        <span>Workspace</span>
      </a-menu-item>
      <a-sub-menu>
        <template #icon>
          <apartment-outlined />
        </template>
        <template #title>Menu</template>
        <a-menu-item key="3">
          <template #icon> <team-outlined /></template>Sub Menu Item
        </a-menu-item>
        <a-menu-item key="4">
          <template #icon> <database-outlined /></template>Sub Menu Item
        </a-menu-item>
        <a-sub-menu>
          <template #icon>
            <apartment-outlined />
          </template>
          <template #title> Sub Menu </template>
          <a-menu-item key="5">
            <template #icon> <team-outlined /></template>Sub Menu Item
          </a-menu-item>
          <a-menu-item key="6">
            <template #icon> <database-outlined /></template>Sub Menu Item
          </a-menu-item>
        </a-sub-menu>
      </a-sub-menu>
      <a-menu-item key="7">
        <template #icon> <login-outlined /></template>
        <router-link to="/login">
          <span>Login Page</span>
        </router-link>
      </a-menu-item>
    </a-menu>
  </a-layout-sider>
</template>

<style lang="scss" scoped>
.logo {
  width: 80%;
  height: 44px;
  background-color: #8297aa6e;
  margin: 12px auto;
}
</style>
