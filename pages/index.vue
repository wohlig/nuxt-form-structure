<template>
  <div class="home-page ">
    <div class="gradientHome">
      <div class="iGradient">
      </div>
      <Header/>
      <Banner/>
    </div>

  </div>
</template>

<script>

import Header from '~/components/header.vue'
import Banner from '~/components/banner.vue'
export default {
  components: {
    Header,
    Banner
  }
}
</script>

<style lang="scss">
.home-page{
  background-repeat: no-repeat;
  background-image: url("~@/assets/Images/office-space.jpg");
  background-attachment: scroll;
  background-position: center center;
  width:100%;
  height: 100vh;
  background-size: cover;
  position: relative;
    .gradientHome{
      min-height: 100vh;
      overflow: hidden;
      position: relative;
    }
    .iGradient{
      position: absolute;
      top: 0;
      right: 0;
      left: 0;
      bottom: 0;
      background-image: linear-gradient(90deg,rgba(48,172,177,.8),rgba(115,173,39,.8));
      z-index: 0;
    }
}
</style>
