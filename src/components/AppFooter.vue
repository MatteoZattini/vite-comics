<script>
	export default {
		data() {
			return {
                footerLinks: [
                    {
                        titolo: "DC COMICS",
                        links: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News",]
                    }, {
                        titolo: "SHOP",
                        links: ["Shop DC", "Shop DC Collectibles"]
                    }, {
                        titolo: "DC",
                        links: ["Term Of Use", "Privacy policy(New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contac Us"],
                    }, {
                        titolo: "SITES",
                        links: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
                    }
                ]
			}
		},

		methods: {

		},

		mounted() {

		}
	}
</script>

<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-6 box-links">
                    
                        <div class="ciaoo" v-for="element, i in footerLinks">
                            <ul class="p-0">
                                <h4>{{ element.titolo }}</h4>
                                <li v-for="link in element.links">{{ link }}</li>
                            </ul>
                        </div>
                    
                </div>
                <div class="col-6">
                    <div class="box-img-bg">

                    </div>
                </div>
            </div>
        </div>
        <div class="container">

        </div>
    </footer>
</template>

<style scoped>
*{
    color: white;
}

footer {
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 23.5rem;
}

.box-links {
    height: 23.5rem;
    padding-top: 2.5rem;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}

.ciaoo {
    width: 10rem;
    max-height: auto;
    margin-bottom: 0.5rem;
}

li {
    list-style: none;
    color: gray;
    font-size: 0.9rem;
}

.box-img-bg {
    width: 100%;
    height: 100%;
    background-image: url(/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position-x: center;
    background-position-y: center;
}
</style>