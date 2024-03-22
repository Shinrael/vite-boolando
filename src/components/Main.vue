<script>
import ProductCard from './partials/ProductCard.vue';
import productsData from './data/db'
  export default {
    data(){
      return{
        products: productsData[0].products
      }
    },
    components:{
      ProductCard
    }
  }
</script>

<template>
  <main>
    <div class="container d-flex flex-wrap justify-content-center align-content-start overflow-hidden">
      <ProductCard 
        v-for="product in products"
        :key="product.id"
        :productImageFront="product.frontImage"
        :productImageBack="product.backImage"
        :productBrand="product.brand"
        :productName="product.name"
        :productPrice="product.price"
      />
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