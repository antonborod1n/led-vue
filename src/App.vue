<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Top from "./components/Top.vue";
import PopularGoods from "./components/PopularGoods.vue";
import ProductBox from "./components/ProductsBox.vue";
</script>

<template>
  <Header />
  <main class="main">
    <Top />
    <PopularGoods />
    <ProductBox />
  </main>
  <Footer />
</template>

<style scoped>
</style>
