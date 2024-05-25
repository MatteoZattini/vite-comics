<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppJumbo from './components/AppJumbotron.vue'
import AppSeries from './components/AppSeries.vue'
import AppPreFooter from './components/AppPreFooter.vue';
import AppFooter from './components/AppFooter.vue';
import AppPostFooter from './components/AppPostFooter.vue';



	export default {
		components: {
			AppHeader,
			AppMain,
			AppJumbo,
			AppSeries,
			AppPreFooter,
			AppFooter,
			AppPostFooter,
		},

		data() {
			return {

			}
		},

		methods: {

		},

		mounted() {

		}
	}
</script>

<template>

<AppHeader />

<AppJumbo />
<AppSeries />
<AppPreFooter />
<AppFooter />
<AppPostFooter />

</template>

<style>
</style>