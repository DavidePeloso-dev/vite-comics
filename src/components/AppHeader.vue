<script>
export default {
    name: 'AppHeader',
    data() {
        return {

        }
    },
    components: {
    },
    methods: {

    },
}
</script>

<template>
    <header>
        <div class="container d-flex justify-content-between align-items-center">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="dc logo">
            </div>
            <nav>
                <ul class="d-flex align-items-center">
                    <li><a href="#">CHARACTERS</a></li>
                    <li><a class="active" href="#">COMICS</a></li>
                    <li><a href="#">MOVIE</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header {
    height: 118px;
    background-color: var(--dc-ligth);
}

.logo {
    width: 100px;
    padding: 0.5rem;
}

nav ul {
    gap: 2rem;

    & a {
        color: var(--dc-dark);
        font-size: 0.8rem;
        font-weight: 700;
        line-height: 118px;
    }

    & .active {
        color: var(--dc-primary);
        border-bottom: 5px solid;
        padding-bottom: 2.85rem;
    }

}
</style>