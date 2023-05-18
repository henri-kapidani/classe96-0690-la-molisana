<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppProducts from './components/AppProducts.vue';
// const AppHeader = valore esportato dal file importato

export default {
	components: { AppHeader, AppProducts, AppFooter },
};
</script>

<template>
	<app-header></app-header>

	<main>
		<app-products></app-products>
	</main>

	<app-footer></app-footer>
</template>

<style lang="scss">
@use './assets/styles/general.scss' as *;
</style>
