<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
    <BottomPage />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import BottomPage from "./components/BottomPage.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
    BottomPage,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
  height: auto;
}

body {
  min-height: 100vh;
}
</style>
