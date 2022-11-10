<script>
export default{
    name: "navBar",
    data(){
        return{
            cards:[
                {
                    url:"../assets/img/buy-comics-digital-comics.png",
                    description:"digital comics"
                },
                {
                    url:"../assets/img/buy-comics-merchandise.png",
                    description:"digital comics"
                },
                {
                    url:"../assets/img/buy-comics-subscriptions.png",
                    description:"digital comics"
                },
                {
                    url:"../assets/img/buy-comics-shop-locator.png",
                    description:"digital comics"
                },
                {
                    url:"../assets/img/buy-dc-power-visa.svg",
                    description:"digital comics"
                },
            ]
        }
    },
    //unico metodo in vue per inserire url
    methods:{
        getImagePath: function(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
    //funzioni
}
</script>

<template>

    <div class="generalCard py-5">
        <div class="container">
            <div class="row rows-col-5 justify-content-center align-items-center">
                <div class="col" v-for="card in cards">
                    <img :src="getImagePath(card.url)" alt="">
                    <span class="text-uppercase text-light px-2">{{card.description}}</span>
                </div>
            </div>
        </div>
    </div>

</template>