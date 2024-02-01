<script>
export default {
    name: "AppFooterBar",
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
    <div class="footer-bar">
        <div class="container d-flex align-items-center justify-content-between">
            <div class="btn">SING-UP NOW!</div>
            <div class="socials d-flex align-items-center gap-3">
                <a href="">FOLLOW US</a>
                <a href="">
                    <img src="/img/footer-facebook.png" alt="">
                </a>
                <a href="">
                    <img src="/img/footer-twitter.png" alt="">
                </a>
                <a href="">
                    <img src="/img/footer-youtube.png" alt="">
                </a>
                <a href="">
                    <img src="/img/footer-pinterest.png" alt="">
                </a>
                <a href="">
                    <img src="/img/footer-periscope.png" alt="">
                </a>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer-bar {
    height: 110px;
    width: 100%;
    background-color: var(--dc-footer-bar);
    z-index: 999;
    position: relative;

    & a {
        color: var(--dc-primary);
        font-weight: 700;
    }
}

.container {
    height: inherit;
}
</style>