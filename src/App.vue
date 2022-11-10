<script>
import navBar from "./components/navBar.vue";
import jumbo from "./components/jumbotron.vue";
import card from "./components/generalCard.vue";

export default{
  name: "app",
  components:{
    navBar,
    jumbo,
    card,
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


</template>

<style scoped>

</style>
