<script setup lang="ts">
import { defineProps, onMounted } from 'vue';
import { useRouter } from 'vue-router';

const curCompProps = defineProps<{ id: string }>();
const curRouter = useRouter();

onMounted(() => {
  const { currentRoute } = curRouter || {};
  const { params } = currentRoute.value || {};
  console.log('params____', params);
});
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
