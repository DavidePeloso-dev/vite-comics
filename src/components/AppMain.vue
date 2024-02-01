<script>
import AppFeatures from './AppFeatures.vue';
export default {
    name: "AppMain",
    data() {
        return {

        }
    },
    components: {
        AppFeatures,
    },
    methods: {

    },
}
</script>

<template>
    <main>
        <div class="container d-flex align-items-center">
            <h3> Content goes here </h3>
        </div>
        <AppFeatures></AppFeatures>
    </main>
</template>

<style scoped>
main {
    background-color: var(--dc-dark);

    & .container {
        height: 118px;
    }
}

h3 {
    color: var(--dc-ligth);
}
</style>