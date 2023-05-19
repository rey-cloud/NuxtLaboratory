<template>
  <div class="card text-center">
    <img :src="product.image" alt="product thumb" class="thumb">
    <p class="font-bold text-gray-500 m-4">{{ product.title }}</p>
    <p class="font-bold text-gray-500 m-4">{{ product.price }}</p>
    <p class="font-bold text-gray-500 m-4">{{ product.category }}</p>
  </div>
</template>

<script setup>
  const { product } = defineProps(['product'])
</script>

<style scoped>
  .thumb {
    max-height: 120px;
    max-width: 70%;
    margin: 0 auto;
  }
</style>