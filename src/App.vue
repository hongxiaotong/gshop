<template>
  <div id="app">
    <router-view />
    <FooterGuide v-show="$route.meta.showFooter"/>
  </div>
</template>

<script>
import FooterGuide from "./components/FooterGuide/FooterGuide.vue";
import {reqCategorys} from "./api/index"
export default {
  data() {
    return {};
  },

  components: {
    FooterGuide
  },

  methods: {}
  // async mounted() {
  //   const result = await reqCategorys()
  //   console.log(result)
  // }
};
</script>

<style lang="stylus" ref="stylesheet/stylus">
.app
  width 100%
  height 100%
  background #f5f5f5
  position relative
</style>