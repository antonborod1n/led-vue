<template>
  <section class="product-box">
    <div class="container">
      <ProductItem />
    </div>
  </section>
</template>

<script setup>
import ProductItem from "./ProductItem.vue";
</script>

<style lang="scss" scoped>
.product-box {
  padding: 57px 0 45px;
}
</style>