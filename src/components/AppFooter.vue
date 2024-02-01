<script>
import AppFooterBar from "./AppFooterBar.vue";

export default {
    name: "AppFooter",
    data() {
        return {

        }
    },
    components: {
        AppFooterBar,
    },
    methods: {

    },
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="wrapper d-flex justify-content-between align-items-center">
                <div class="lists d-flex gap-5">
                    <div class="list">
                        <ul>
                            <h3>DC COMICS</h3>
                            <li><a href="">Characters</a></li>
                            <li><a href="">Comics</a></li>
                            <li><a href="">Movie</a></li>
                            <li><a href="">TV</a></li>
                            <li><a href="">Games</a></li>
                            <li><a href="">Videos</a></li>
                            <li><a href="">News</a></li>
                        </ul>
                        <ul>
                            <h3>SHOP</h3>
                            <li><a href="">Shop DC</a></li>
                            <li><a href="">Shop DC Collections</a></li>
                        </ul>
                    </div>
                    <div class="list">
                        <ul>
                            <h3>DC</h3>
                            <li><a href="">Terms Of Use</a></li>
                            <li><a href="">Privacy Policy (New)</a></li>
                            <li><a href="">Ad Choices</a></li>
                            <li><a href="">Advertising</a></li>
                            <li><a href="">Jobs</a></li>
                            <li><a href="">Subscriptions</a></li>
                            <li><a href="">Talent Workshops</a></li>
                            <li><a href="">CPSC Certificates</a></li>
                            <li><a href="">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="list">
                        <ul>
                            <h3>SITES</h3>
                            <li><a href="">DC</a></li>
                            <li><a href="">MAD Magazine</a></li>
                            <li><a href="">DC Kids</a></li>
                            <li><a href="">DC Universe</a></li>
                            <li><a href="">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
                <div class="logo">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <AppFooterBar></AppFooterBar>
    </footer>
</template>

<style scoped>
footer {
    background-image: url(/img/footer-bg.jpg);

}

h3 {
    color: var(--dc-ligth);
    font-weight: 700;
    padding: 2rem 0 0.5rem;
}

ul a {
    color: var(--dc-secondary);
    line-height: 1.5rem;
}

.wrapper {
    position: relative;
    padding: 3rem 0;
}

.logo {
    width: 50%;
    position: absolute;
    right: 0;
}
</style>