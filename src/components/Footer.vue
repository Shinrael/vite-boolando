<script>
  export default {
    data(){
      return{
        informations:[
          {
            title:'Informazioni Legali',
            link: '#',
          },
          {
            title:'Informativa sulla privacy',
            link: '#',
          },
          {
            title:'Diritto di recesso',
            link: '#',
          },
        ],
        icons:[
          {
            img:'<i class="fa-brands fa-square-twitter"></i>',
            link: '#'
          },
          {
            img:'<i class="fa-brands fa-square-facebook"></i>',
            link: '#'
          },
          {
            img:'<i class="fa-brands fa-square-instagram"></i>',
            link: '#'
          },
          {
            img:'<i class="fa-brands fa-square-pinterest"></i>',
            link: '#'
          },
          {
            img:'<i class="fa-brands fa-square-youtube"></i>',
            link: '#'
          },
        ]
      }
    }
  }
</script>

<template>
  <footer class="d-flex align-items-center justify-content-center">
    <div class="main-wrapper d-flex">
      <div class="left d-flex flex-column">
      <h5>Boolando S.R.L.</h5>
      <ul class="d-flex list-unstyled ">
        <li v-for="(info,index) in informations" :key="index">
          <a href="info.link">{{ info.title }}</a>
        </li>
      </ul>
      </div>
      <div class="right d-flex flex-column align-items-end ">
        <h6>Trovaci anche su</h6>
        <ul  class="d-flex list-unstyled">
          <li v-for="(icon,index) in icons" :key="index">
            <a href="icon.link" v-html="icon.img"></a>
          </li>
        </ul>
      </div>  
    </div>
  </footer>
</template>



<style lang="scss" scoped>

@use '../assets/scss/partials/variables' as*;

footer{
  height: 115px;
  background-color: $bg-color-footer;
  color: $color-font;
  .main-wrapper{
    width: 80%;
    .left{
    width: 50%;
    h5{
      font-weight: bold;
    }
    ul{
      li{
        padding: 0 15px 0 0;
        a{
          text-decoration: none;
          color: $color-font;
        }
      }
    }
  }
  .right{
    width: 50%;
    h6{
      font-weight: bold;
    }
    ul{
      li{
        padding: 0px 5px; 
        font-size: 1.3rem;
        a{
          color: $color-font;          
        }
      }
    }
  }
  }
  
}
</style>