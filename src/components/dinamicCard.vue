<script>
export default {
    name: "dinamicCard",
    props: {
        image: String,
        title: String
    }
}
</script>

<template>

    <div class="col my-3">
        <img :src="image" alt="">
        <p class="text-light mt-2 text-uppercase text-center">{{ title }}</p>
    </div>

</template>