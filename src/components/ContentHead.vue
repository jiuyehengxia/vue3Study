<script setup lang="ts">
import { defineProps } from 'vue'

defineProps<{ headTitle: string }>()
</script>

<template>
  <div class="head-wrap">
    <div class="head-title">{{ headTitle }}</div>
    <div class="head-bottom">
      <div class="bottom-left"></div>
      <div class="bottom-right"></div>
    </div>
  </div>
</template>

<style scoped>
.head-wrap .head-title {
  color: #5858e5;
  height: 36px;
  line-height: 36px;
  font-weight: 600;
}
.head-wrap .head-bottom {
  width: 100%;
  height: 4px;
  background: #eee;
}
.head-wrap .head-bottom .bottom-left {
  width: 20mm;
  height: 100%;
  background: #5858e5;
}
</style>
