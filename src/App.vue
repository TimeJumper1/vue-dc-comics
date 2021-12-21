<template>
  <div id="app">
    <Header />
    <main>
      <Main />
    </main>
    <prefooter />
    <footer-banner />
    <Footer />
    
  </div>
</template>

<script>

import Header from "./components/header.vue";
import Main from "./components/main.vue";
import prefooter from "./components/prefooter.vue";
import footerBanner from "./components/footer-banner.vue";
import Footer from "./components/footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    prefooter,
    footerBanner,
    Footer,
  },
};
</script>

<style lang="scss">
 *{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
ul{
  list-style-type: none;

}
a{
  text-decoration: none;
}
</style>
