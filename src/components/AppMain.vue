<script>
import AppFeatures from './AppFeatures.vue';
import AppComic from "./AppComic.vue";
export default {
    name: "AppMain",
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://th.bing.com/th/id/OIP.qLTi11FsVESAP0oVhXupIAHaLY?pid=ImgDet&w=84&h=84&c=7&dpr=2",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://3.bp.blogspot.com/-EwBcReCXtLM/WajhuVz__sI/AAAAAAABQNY/Vd5VTYt7qOgUSwm7tLBba35MNNPm7pGOwCLcBGAs/s1600/042_0000.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://th.bing.com/th/id/OIP.lyDSKMYRPpS7xh9JPBwsowHaLZ?pid=ImgDet&w=84&h=84&c=7&dpr=2",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://th.bing.com/th/id/OIP.6ag3YF2rFWwe1aSpvLcOaAHaLY?pid=ImgDet&w=192&h=294&c=7&dpr=2",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://th.bing.com/th/id/OIP.DuBSOXdSPlc0KDT0kAT3XQHaLF?pid=ImgDet&w=84&h=84&c=7&dpr=2",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://th.bing.com/th/id/OIP.gWVQEk5Lg0ZpWZJi5dIXxwHaLY?pid=ImgDet&w=84&h=84&c=7&dpr=2",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://th.bing.com/th/id/OIP.pPz23KhyPgekZL5uA7AGJQHaLL?pid=ImgDet&w=84&h=84&c=7&dpr=2",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
        }
    },
    components: {
        AppFeatures,
        AppComic,
    },
    methods: {

    },
}
</script>

<template>
    <main>
        <div class="hero">
            <img src="/img/jumbotron.jpg" alt="">
        </div>
        <div class="container d-flex align-items-center">
            <div class="badge">CURRENT SERIES</div>
            <div class="shelves d-flex justify-content-center flex-wrap">
                <div class="card col-2" v-for="comic in comics">
                    <AppComic :src="comic.thumb" :title="comic.series"></AppComic>
                </div>
                <div class="btn">LOAD MORE</div>
            </div>
        </div>
        <AppFeatures></AppFeatures>
    </main>
</template>

<style scoped>
main {
    background-color: var(--dc-dark);

    & .container {
        padding: 2rem 0;
    }
}

.hero img {
    height: 400px;
    object-fit: cover;
    object-position: 0 0;
}


h3 {
    color: var(--dc-ligth);
}

.card {
    padding: 1rem;
}

.shelves {
    margin: 0 -1rem;
}

.btn,
.badge {
    padding: 0.5rem 2.5rem;
    background-color: var(--dc-primary);
    font-size: 0.8rem;
    font-weight: 700;
}

.container {
    position: relative;
}

.badge {
    position: absolute;
    left: 0;
    top: 0;
    translate: 0 -50%;
    font-size: 1rem;
}
</style>