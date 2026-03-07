<script setup lang="ts">
import { LeftMenu } from '@/components'
</script>

<template>
  <div class="setting-hone">
    <div class="setting-hone-menu">
      <LeftMenu />
    </div>
    <div class="w-full setting-hone-content">
      <router-view />
    </div>
  </div>
</template>

<style lang="less" scoped>
.setting-hone {
  height: 100vh;
  display: flex;
  &-menu {
    height: 100%;
    min-height: 0;
  }

  &-content {
    flex: 1;
    min-height: 0;
    overflow: hidden;
  }
}
</style>
