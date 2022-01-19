<template>
  <div id="app">

    <header>

      <Header :headerD = headerData />

    </header>

    <main>

    <Main />

    </main>

    <footer>

      <Footer :footerD = footerData />

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

      footerData: {

        footerDataLinkOne: ["Request a website", "Browse Themes", "Payment option", "Support System", "Checkout", "Purchase Theme"],
        footerDataLinkTwo: ["Purchase Theme", "Our Benefits", "Our Team", "Our Services", "Other Products", "My Account"],
        footerDataCategories: ["Economy", "Design", "Coaching", "Business", "Medicine", "Law", "Fitness"],

      }

    }

  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Architects+Daughter&family=Roboto:wght@300&display=swap');

#app{

  overflow: hidden;

  font-family: 'Architects Daughter', cursive;
  font-family: 'Roboto', sans-serif;

}

</style>
