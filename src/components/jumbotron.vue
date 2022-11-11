<script>
import AppDinamicCard from "./AppDinamicCard.vue";
export default {
    name: "jumbotron",
    components:{
        AppDinamicCard,
    }
}
</script>

<template>

    <div class="jumbo"></div>
    <div class="bg-dark py-5">
        <AppDinamicCard/>
    </div>


</template>

<style lang="scss">
.jumbo {
    height: 600px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}
</style>