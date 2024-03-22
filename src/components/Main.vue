<script>
import ProductCard from './partials/ProductCard.vue';
  export default {
    components:{
      ProductCard
    }
  }
</script>

<template>
  <main>
    <div class="container d-flex flex-wrap justify-content-center align-content-start overflow-hidden">
      <ProductCard />
      <ProductCard />
      <ProductCard />
      <ProductCard />
      <ProductCard />
      <ProductCard />

    </div>
  </main>
</template>



<style lang="scss" scoped>
main{
  height: 100%;
  .container{
    width: 80%;
    max-width: 1000 px;
    margin: 40px auto;
  }
}
</style>