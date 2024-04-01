<script setup lang="ts">
import { ref, defineProps, onMounted } from 'vue';

defineProps<{
  msg: string;
}>();

const count = ref(0);

const handleBtnClick = () => {
  count.value = count.value + 1;
};

onMounted(() => {
  console.log('count______________', count.value);
});
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
  </div>
  <div>
    <button @click="handleBtnClick">点击次数 {{ count }}</button>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
