<script setup>
import Header from './components/Header.vue'
import Counter from './components/Counter.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Header />
  <main class="container">
    <Counter />
  </main>
  <Footer />
</template>

<style scoped>
main {
  display: flex;
  align-items: center;
  justify-content: center;
  height: calc(100vh - 50px - 50px);
}
</style>
