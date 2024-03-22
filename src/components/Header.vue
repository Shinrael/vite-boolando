<script>
  export default {
    data(){
      return{
        menu:[
          {
            title: 'Donna',
            link: '#',
          },
          {
            title: 'Uomo',
            link: '#',
          },
          {
            title: 'Bambino',
            link: '#',
          },
        ],
        icons:[
          {
            img: '<i class="fa-regular fa-user"></i>',
            link: '#',
          },
          {
            img: '<i class="fa-regular fa-heart"></i>',
            link: '#',
          },
          {
            img: '<i class="fa-solid fa-bag-shopping"></i>',
            link: '#',
          },
        ]
      }
    }
  }
</script>

<template>
  <header class="d-flex justify-content-center">
    <div class="main-wrapper d-flex justify-content-around align-items-center">
      <div class="menu d-flex">
      <ul class="d-flex list-unstyled align-items-center">
        <li v-for="(item,index) in menu" :key="index">
          <a href="item.link">{{ item.title }}</a>
        </li>        
      </ul>
    </div>
    <div class="logo d-flex align-items-center justify-content-center">
      <div class="img-container">
        <img src="/public/boolean-logo.png" alt="logo">
      </div>
    </div>
    <div class="icon d-flex align-items-center justify-content-end">
      <ul class="d-flex list-unstyled align-items-center">
        <li v-for="(icon,index) in icons" :key="index">
          <a href="icon.link" v-html="icon.img"></a>
        </li>
      </ul>
    </div>
    </div>
  </header>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as*;

header{
  height: 70px;
  background-color: $bg-color-header;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.5);
  .main-wrapper{
    width: 80%;
    .menu{
    width: 33%;
    ul{
      margin-top: 10px;
      li{
        padding: 0px 10px;        
        font-weight: bold;
        a{
          color: $color-font;
          text-decoration: none;
        }
      }
    }
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
    ul{
      margin-top: 10px;
      li{
        padding: 0px 10px; 
        a{
      color: $color-font
    }
      }
    }
    
  }
}
  }
  
</style>