<template>
  <div id="app">
    <router-view />
    <!-- 当前路由$route -->
      <FooterGuide v-show="$route.meta.showFooter"/>
  </div>
</template>

<script>
import FooterGuide from "./components/FooterGuide/FooterGuide.vue";
export default {
  components: {
    FooterGuide
  },
  name: "App"
};
</script>

<style lang="stylus" rel="stylesheet/stylus">
  #app
    width 100%
    height 100%
    position relative
</style>

