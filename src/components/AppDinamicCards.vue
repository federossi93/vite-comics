<script>
import seriesObject from "../data/dc-comics.js";
import cardSeries from "./dinamicCard.vue"
export default {
    name: "AppDinamicCards",
    components: {
        cardSeries,
    },
    data() {
        return {
            single: seriesObject
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="row rows-col-6 ">
            <cardSeries v-for="poster in single" :image="poster.thumb" :title="poster.series" />
        </div>
        <!-- <div class="row rows-col-6 ">
            <div class="col my-3" v-for="poster in single">
                <img :src="poster.thumb" alt="">
                <p class="text-light mt-2 text-uppercase text-center">{{poster.series}}</p>
            </div>
        </div> -->

        <div class="text-center">
            <button type="button" class="btn btn-primary text-uppercase px-5">load more</button>
        </div>
    </div>
</template>