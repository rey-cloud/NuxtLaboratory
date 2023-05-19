<template>
  <div>
    <header class="">
      <nav>
        <ul class="flex">
          <li class="mx-10 my-10 font-bold"><nuxt-link to="/">Home</nuxt-link></li>
          <li class="mx-10 my-10 font-bold"><nuxt-link to="/products">Products</nuxt-link></li>
        </ul>
      </nav>
    </header>

    <div>
      <slot />
    </div>
  </div>
</template>

<style scoped>
  .router-link-exact-active {
    color:chartreuse;
  }
</style>