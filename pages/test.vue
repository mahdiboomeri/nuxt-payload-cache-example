<template>
  <button @click="log('posts')">Log the data</button>
</template>

<script setup lang="ts">
const log = (key: string) => {
  console.log(useNuxtApp().payload.data[key]);
};
</script>
