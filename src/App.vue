<template>
  <div id="app">

    <header>

      <Header :headerD = headerData />

    </header>

    <main>

    <Main />

    </main>

    <footer>

      <Footer />

    </footer>

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import "./assets/general.scss";
import "./assets/color.scss";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
  data(){

    return {

      headerData: {

          headerDataInfo: ["Home", "Courses", "About Us", "News", "Pages"],

          headerDataCourses: ["Contact", "Purchase"],

        },

    }

  },
};
</script>

<style lang="scss">

</style>
