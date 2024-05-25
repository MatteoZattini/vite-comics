<script>
	export default {
		data() {
			return {
                 fumetti: [
    {
        thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
        price: "$19.99",
        series: "Action Comics",
        type: "comic book",
    },
    {
        thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
        price: "$3.99",
        series: "American Vampire 1976",
        type: "comic book",
    },
    {
        thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
        price: "$16.99",
        series: "Aquaman",
        type: "graphic novel",
    },
    {
        thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
        price: "$2.99",
        series: "Batgirl",
        type: "comic book",
    },
    {
        thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
        price: "$3.99",
        series: "Batman",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
        price: "$2.99",
        series: "Batman Beyond",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
        price: "$3.99",
        series: "Batman/Superman",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
        price: "$4.99",
        series: "Batman/Superman Annual",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
        price: "$5.99",
        series: "Batman: The Joker War Zone",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
        price: "$6.99",
        series: "Batman: Three Jokers",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
        price: "$4.99",
        series: "Batman: White Knight Presents: Harley Quinn",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
        price: "$16.99",
        series: "Catwoman",
        type: "graphic novel",
    },
]
			}
		},

		methods: {
            getImagePath: function(img) {
                return new URL(`/img/${img}`, import.meta.url).href;
            }
		},

		mounted() {

		}
	}
</script>

<template>
<main>
    <div class="container h-100 position-relative">
        <button class="button2">CURRENT SERIES</button>
            <div class="col-12 h-100 d-flex flex-wrap justify-content-center">
                <div v-for="element in fumetti" class="mycard">
                    <img class="object-fit-cover" :src="element.thumb" alt="">
                    <span>{{ element.series }}</span>
                </div>

                <button class="button1">LOAD MORE</button>
            </div>
        
    </div>
</main>
</template>

<style scoped>
*{
    color: white;
}

main {
    width: 100%;
    height: 35rem;
    background-color: #222;
}

img {
    width: 100%;
    height: 100%;
    object-position: top;
}

.col-12 {
    padding-top: 5rem;
}

.mycard {
    width: calc(100% / 6 - 2rem);
    height: 10rem;
    margin: 0 1rem;

}

.button1 {
	color: white;
    border: none;
	padding: 0.8rem 0.8rem;
	background: #0282f9;
	font-weight: bold;
    height: 3rem;
}

.button2 {
    position: absolute;
    top: -30px;
    font-size: 1.5rem;
	color: white;
    border: none;
	padding: 0.8rem 0.8rem;
	background: #0282f9;
	font-weight: bold;
}
</style>