<script>
export default {
    name: "AppFeatures",
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
    <div class="wrapper">
        <div class="container">
            <div class="links d-flex align-items-center justify-content-around">
                <div class="link d-flex align-items-center">
                    <div class="icon">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <a href="">DIGITAL COMICS</a>
                </div>
                <div class="link d-flex align-items-center">
                    <div class="icon">
                        <img src="/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <a href="">DC MERCHANDISE</a>
                </div>
                <div class="link d-flex align-items-center">
                    <div class="icon">
                        <img src="/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <a href="">SUBSCRIPTION</a>
                </div>
                <div class="link d-flex align-items-center">
                    <div class="icon">
                        <img src="/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <a href="">COMICS SHOP LOCATOR</a>
                </div>
                <div class="link d-flex align-items-center">
                    <div class="icon">
                        <img src="/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <a href="">DC POWER VISA</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.wrapper {
    height: 118px;
    width: 100%;
    background-color: var(--dc-primary);
}

.links {
    height: inherit;
}

.link a {
    color: var(--dc-ligth);
    font-size: 0.8rem;
}

.icon {
    width: 3rem;
    padding-right: 1rem;
}

.container {
    height: 118px;
}
</style>