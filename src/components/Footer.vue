<script>
  export default {
    
  }
</script>

<template>
  <footer class="d-flex align-items-center">
    <div class="left d-flex flex-column">
      <h5>Boolando S.R.L.</h5>
      <ul class="d-flex list-unstyled ">
        <li><a href="#">Informazioni Legali</a></li>
        <li><a href="#">Informativa sulla privacy</a></li>
        <li><a href="#">Diritto di recesso</a></li>
      </ul>
    </div>
    <div class="right">

    </div>
  </footer>
</template>



<style lang="scss" scoped>

@use '../assets/scss/partials/variables' as*;

footer{
  height: 115px;
  background-color: $bg-color-footer;
  color: $color-font;
  .left{
    width: 50%;
    padding-left: 180px;
    ul{
      li{
        padding: 0 10px;
        a{
          text-decoration: none;
          color: $color-font;
        }
      }
    }
  }
  .right{
    width: 50%;
  }
}
</style>