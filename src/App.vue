<script setup>
import BlogCard from './components/BlogCard.vue';
</script>

<template>
  <header>
    <h1>Blog Card</h1>
  </header>
  <main>
    <div class="container">
      <BlogCard />
    </div>
  </main>
</template>

<style scoped lang="scss">
header {
  & h1 {
    display: none;
  }
}

main {
  & .container {
    margin: 0 var(--spacing200);
  }
}

</style>
