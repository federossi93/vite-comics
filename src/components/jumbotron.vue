<script>
import AppDinamicCard from "./AppDinamicCards.vue";
export default {
    name: "jumbotron",
    components: {
        AppDinamicCard,
    }
}
</script>

<template>

    <div class="jumbo">
        <div class="content btn bg-primary text-light text-uppercase px-5">content series</div>
    </div>

    <div class="bg-dark py-5">

        <AppDinamicCard />

        
    </div>


</template>

<style lang="scss">
.jumbo {
    
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    .content{
        margin-top: 400px;
        margin-bottom: -20px;
        margin-left: 200px;
        
    }
}
</style>