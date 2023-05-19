<template>
  <div>
    <div class="grid grid-cols-3 gap-5 mx-64">
      <div v-for="p in products">
        <ProductCard :product="p" />
      </div>
    </div>
  </div>
</template>

<script setup>
  const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>

</style>