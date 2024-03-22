<script>
  export default {
    props:{
      productImageFront: String,
      productImageBack: String,
      productBrand: String,
      productName: String,
      productPrice: String
    }
    
  }
</script>


<template>
  <div class="product">
      <img class="image-one" :src="productImageFront" alt="Vestito">
      <img class="image-two" :src="productImageBack" alt="Vestito Alt">
      <div class="product-text">
        <p>{{ productBrand }}</p>
        <p><strong>{{ productName }}</strong></p>
        <p><span class="price-now">14,99 &euro;</span> <span class="first-price">{{ productPrice }} &euro;</span></p>
      </div>
      <div class="discount">-50%</div>
      <div class="green">Sostenibilità</div>
      <div class="heart"><i class="fa-solid fa-heart"></i>        
      </div>
  </div>
</template>



<style lang="scss" scoped>
      .product{
      margin: 0px 6px 25px;
      position: relative;
      width: 32%;
      height: 520px;
      cursor: pointer;
      &:hover{
        .image-one{
          display: none;
        }
        .image-two{
          display: block;
        }
      }
      .image-two{
        display: none;
      }
      img{
        width: 100%;
        height: auto;
      }
      .product-text{
        position: absolute;
        left: 0;
        bottom: 0;
        .price-now{
          color: red;
        }
        .first-price{
          text-decoration: line-through;
        }
      }
      .discount{
        position: absolute;
        bottom: 80px;
        left: 0;
        color: white;
        padding: 4px 9px;
        background-color: red;
      }
      .discount-light{
        position: absolute;
        bottom: 80px;
        left: 0;
        color: white;
        padding: 4px 9px;
        background-color: red;
      }
      .green{
        position: absolute;
        bottom: 80px;
        left: 56px;
        color: white;
        padding: 4px 9px;
        background-color: #008000;
      }  
      .green-alt{
        position: absolute;
        bottom: 80px;
        left: 0;
      }
      .heart{
        position:absolute;
        top: 5px;
        right:0px;
        padding: 12px 12px;
        background-color: white;
        size: 1px;
        &:hover{
          color: red;
        }
      }
        
    }
</style>