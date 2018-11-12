<template>
  <div class="home" :style="{ backgroundImage: `url(${backGroundUrl})` }">
    <div class="opacitybg">
    <h1 class="logoHome"><img src="~/assets/img/home/home_logo.png" alt=""></h1>
    <p class="homelink"><nuxt-link class="btn_content" to="/mainMenu">Customer Support</nuxt-link></p>
    </div>
  </div>
  
</template>

<script>
import backGroundUrl from "~/assets/img/home/bg_home.jpg"
export default {
  data() {
    return { backGroundUrl }
  }
  
}
</script>

<style scoped>
  .home {
    background-repeat: no-repeat;
    background-position: center; 
    background-size: cover;
    height: 825px;
  }
  .logoHome {
    margin: 0 auto;
    padding: 250px 0 20px 0;
    width: 300px;
  }
  .logoHome img{
    width: 100%;
  }
  .btn_content {
    color: #fff;
    padding: 10px 15px;
    text-decoration: none;
    display: block;
  }
  .homelink {
    margin: 0 auto;
    border: 2px solid #fff;
    width: 166px;
    border-radius: 50px;
    background: #da0019;
  }
  .opacitybg {
    background:rgba(255, 255, 255, 0.5);
    width: 100%;
    height: 100%;
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0; 
  }
</style>
