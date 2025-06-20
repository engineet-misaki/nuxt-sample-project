<template>
  <nav>
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/about">About</NuxtLink>
    <NuxtLink to="/posts">Post</NuxtLink>
    <NuxtLink to="/posts/catch">Post catch</NuxtLink>
    <NuxtLink :to="{ name: 'users-list' }">User List</NuxtLink>
  </nav>
</template>