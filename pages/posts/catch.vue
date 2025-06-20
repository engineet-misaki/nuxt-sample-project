<script setup>
const { data: posts, error } = await useAsyncData('posts', () =>
  $fetch('https://jsonplaceholder.typicode.com/posts/')
);
</script>
<template>
  <div>
    <h1>Posts一覧 useAsyncData</h1>
    <p v-if="error">{{ error }}</p>
    <ul>
      <li v-for="post in posts" :key="post.id">{{ post.title }}</li>
    </ul>
  </div>
</template>