<template>
  <div id="app">
    <Header />
    <Main />
    <prefooter />
    <footer-banner />
    <footer />
    
  </div>
</template>

<script>

import Header from "./components/header.vue";
import Main from "./components/main.vue";
import prefooter from "./components/prefooter.vue";
import footerBanner from "./components/footer-banner.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    prefooter,
    footerBanner,
  },
};
</script>

<style lang="scss">
 *{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
