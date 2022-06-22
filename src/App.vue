<template>
  <div id="app">
    <TheHeader/>
    <JumbotronImage/>
    <BannerBlack/>
    <BannerBlue/>
    <TheFooter/>
    <BannerSignUp/>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import BannerSignUp from "./components/BannerSignUp.vue";
import BannerBlack from "./components/BannerBlack.vue";
import BannerBlue from "./components/BannerBlue.vue";
import JumbotronImage from "./components/JumbotronImage.vue"

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BannerSignUp,
    BannerBlack,
    BannerBlue,
    JumbotronImage,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
