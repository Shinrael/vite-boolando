<script>
  export default {
    
  }
</script>

<template>
  <header class="d-flex justify-content-around align-items-center">
    <div class="menu d-flex align-items-center justify-content-center">AAA</div>
    <div class="logo d-flex align-items-center justify-content-center">
      <div class="img-container">
        <img src="/public/boolean-logo.png" alt="logo">
      </div>
    </div>
    <div class="icon d-flex align-items-center justify-content-center">AAA</div>
  </header>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as*;

header{
  height: 70px;
  background-color: $bg-color-header;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.5);
  .menu{
    width: 33%;
  }
  .logo{
    width: 33%;
    height: 100%;
    
    .img-container{
      width: 180px;
      height: 40px;
      
      img{
        object-fit: cover;
        width: 100%;
        height: 100%;
      }
    }
  }
  .icon{
    width: 33%;
  }
}
</style>