<script>
import navBar from "./components/navBar.vue";
import jumbo from "./components/jumbotron.vue";

export default{
  name: "app",
  components:{
    navBar,
    jumbo,
  }
}
</script>

<template>
  <navBar/>

  <jumbo/>

</template>

<style scoped>

</style>
