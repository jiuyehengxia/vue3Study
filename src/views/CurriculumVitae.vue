<script setup lang="ts"></script>

<template>
  <div class="outer-wrap">
    <div class="header-area">实事求是，敢为人先</div>
    <div class="content-warp"></div>
  </div>
</template>

<style scoped>
.outer-wrap {
  border: 1px solid #ccc;
  width: 210mm;
  height: 100vh;
  overflow-y: auto;
  padding: 0 20mm;
}
.outer-wrap .header-area {
  color: #333;
  font-size: 24px;
  padding: 6mm 0;
  text-align: center;
  font-family: 'Microsoft YaHei UI';
  position: relative;
}
.outer-wrap .header-area::before {
  position: absolute;
  content: '';
  width: 30px;
  height: 30px;
  border-width: 0 1px 1px 0;
  border-style: solid;
  border-color: #ccc;
  left: -16mm;
  bottom: 0;
}
.outer-wrap .header-area::after {
  position: absolute;
  content: '';
  width: 30px;
  height: 30px;
  border-width: 0 0 1px 1px;
  border-style: solid;
  border-color: #ccc;
  right: -16mm;
  bottom: 0;
}
.outer-wrap .content-warp {
  height: 297mm;
}
</style>
