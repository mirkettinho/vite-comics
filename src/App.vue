
<script>
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import Section from "./components/Section.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components:{
    Header,
    Main,
    Section,
    Footer
  }
}

</script>

<template>
  
  <Header />

  <Main />

  <Section />

  <Footer/>

</template>

<!-- SCSS -->
<style lang="scss">
  // STILI GENERALI

  @use "./scss/main.scss"
</style>