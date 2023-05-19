<script>
import NavBar from './NavBar.vue';

export default {
	data() {
		return {
			logoImgName: 'la-molisana-logo.png',
		};
	},
	methods: {
		getImagePath(img) {
			return new URL(`../assets/img/${img}`, import.meta.url).href;
		},
	},
	components: {
		NavBar,
	},
};
</script>

<template>
	<header>
		<h1 class="text-danger">La molisana</h1>
		<img :src="getImagePath(logoImgName)" alt="" />
		<NavBar />
	</header>
</template>

<style lang="scss" scoped>
@use './../assets/styles/partials/variables' as *;

header {
	text-align: center;
}
</style>
