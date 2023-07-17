<script setup>
const linkUrl = 'https://www.google.com'
const imageUrl = 'https://picsum.photos/seed/picsum/200/300'
</script>

<template>
  <div>
    <img :src="imageUrl" alt="My Image" />
  </div>
  <div>
    <a :href="linkUrl">Click me</a>
  </div>
</template>

<style scoped>

</style>
