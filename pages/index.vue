<template>
  <NuxtLink href="/test">Go to page</NuxtLink>

  <br />

  Hello
</template>

<script setup lang="ts">
const { data } = await useAsyncData("posts", () => $fetch("/api/hello"));
</script>
