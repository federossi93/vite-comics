<script>
import seriesObject from "../data/dc-comics.js";
export default {
    name: "AppDinamicCard",
    data(){
        return{
           single: seriesObject
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="row rows-col-6 ">
            <div class="col" v-for="poster in single">
                <img :src="poster.thumb" alt="">
                <h4 class="text-light mt-2 text-uppercase">{{poster.series}}</h4>
            </div>
        </div>
    </div>
</template>