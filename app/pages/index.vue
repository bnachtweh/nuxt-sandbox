<script setup lang="ts">
const { status, data } = useFetch<Todo>(
  "https://jsonplaceholder.typicode.com/todos/1"
);
</script>

<template>
  <div>
    <h1>{{ status }}</h1>
    <div>{{ data?.title }}</div>
  </div>
</template>
