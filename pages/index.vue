<script setup>
const ctx = useRuntimeConfig();

const { data } = await useFetch("/blog", {
  baseURL: ctx.baseURL,
  headers: {
    "X-MICROCMS-API-KEY": ctx.apiKey,
  },
});
</script>

<template>
  <div>
    <h1>合同会社わしら<small>（仮）</small></h1>
  </div>
</template>
