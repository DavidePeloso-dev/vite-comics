<script>
export default {
    name: "AppComic",
    data() {
        return {

        }
    },
    components: {
    },
    methods: {

    },
    props: {
        src: String,
        title: String,
    }
}
</script>

<template>
    <div class="comic">
        <img :src="src" alt="">
    </div>
    <h4>{{ title }}</h4>
</template>

<style scoped>
.comic {

    & img {
        aspect-ratio: 1;
        object-fit: cover;
        object-position: 0 0;
    }
}

h4 {
    font-weight: 400;

}
</style>