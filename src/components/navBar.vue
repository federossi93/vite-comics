<script>
export default{
    name: "navBar",
    data(){
        return{
            list:[
                {
                    text: "Characters",
                    href: "#"
                },
                {
                    text: "comics",
                    href: "#"
                },
                {
                    text: "movies",
                    href: "#"
                },
                {
                    text: "tv",
                    href: "#"
                },
                {
                    text: "games",
                    href: "#"
                },
                {
                    text: "collectibles",
                    href: "#"
                },
                {
                    text: "videos",
                    href: "#"
                },
                {
                    text: "fans",
                    href: "#"
                },
                {
                    text: "nevs",
                    href: "#"
                },
                {
                    text: "shop",
                    href: "#"
                },
            ]
        }
    },
    //funzioni
}
</script>

<template>
    <div class="container">
        <nav class="navbar d-flex">
            <div>
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div>
                <ul class="d-flex gap-4">
                    <li v-for="element in list">
                        <a 
                        :class="element.text == 'movies' ? 'active' : '' " 
                        :href="element.href">
                        {{element.text}}
                        </a>
                    </li>
                </ul>
            </div>
        </nav>
    </div>

</template>