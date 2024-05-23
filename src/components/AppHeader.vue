<script>
	export default {
		data() {
			return {
				headerLinks: [
					"CHARACTERS",
					"COMICS",
					"MOVIES",
					"TV",
					"GAMES",
					"COLLECTIBLES",
					"VIDEOS",
					"FANS",
					"NEWS",
					"SHOP",
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
	<header>
		<div class="container">
			<div class="row">
				<div class="col-4 d-flex justify-content-between align-items-center">
					<img src="/img/dc-logo.png" alt="">
				</div>
				<div class="col-8 d-flex justify-content-between align-items-center">
					<a v-for="links in headerLinks" href="">{{ links }}</a>
				</div>
			</div>
		</div>
	</header>
</template>

<style scoped>
*{
	font-size: 0.8rem;
}

.row{
	height: 8rem;
}

img{
	width: 5rem;
}

a {
	display: flex;
	justify-content: center;
	align-items: center;
	height: 100%;
	text-decoration: none;
	color: black;
	font-weight: bold;
}

a:hover {
	color: #0282f9;
	border-bottom: 4px solid #0282f9;
}
</style>