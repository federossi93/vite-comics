<script>
import navBar from "./components/navBar.vue";
import jumbo from "./components/jumbotron.vue";
import card from "./components/generalCard.vue";
import foterTop from "./components/footerTop.vue";
import foterBot from "./components/footerBot.vue";

export default{
  name: "app",
  components:{
    navBar,
    jumbo,
    card,
    foterTop,
    foterBot,
  }
}
</script>

<template>

  <header>
    <navBar/>
    <jumbo/>
  </header>

  <main>
    <card/>
  </main>

  <footer>
    <foterTop/>
    <foterBot/>
  </footer>


</template>

<style scoped>

</style>
