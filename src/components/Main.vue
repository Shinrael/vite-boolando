<script>
  export default {
    
  }
</script>

<template>
  <main>
    <div class="container d-flex flex-wrap justify-content-center align-content-start overflow-hidden ">
      <div class="product">
        <img class="image-one" src="" alt="Vestito">
        <img class="image-two" src="" alt="Vestito Alt">
        <div class="product-text">
        <p>Levi's</p>
        <p><strong>RELAXED FIT TEE UNISEX</strong></p>
        <p><span class="price-now">14,99 &euro;</span> <span class="first-price">29,99 &euro;</span></p>
        </div>
        <div class="discount">-50%</div>
        <div class="green">Sostenibilità</div>
        <div class="heart"><i class="fa-solid fa-heart"></i>
        
      </div>
      </div>
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
  }
}
</style>