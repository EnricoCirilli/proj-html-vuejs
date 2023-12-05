<script>
// Header component import
import Header from "./components/Header.vue";
// Main component import
import Main from "./components/Main/Main.vue";
//Footer component import
import Footer from "./components/Footer/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};

</script>

<template>
 <div id="app">
    <!-- Header -->
    <Header />
    <!-- Main -->
    <Main />
    <!-- Footer -->
    <Footer />
  </div>
</template>

<style lang="scss">
@use "./style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";
</style>
