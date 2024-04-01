<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <header>
    <div class="nav-wrap">
      <nav>
        <RouterLink to="/">首页</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <!--        <RouterLink to="/curriculumVitae">简历</RouterLink>-->
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style lang="less" scoped>
.nav-wrap {
  nav a {
    margin-right: 18px;
  }
}
</style>
