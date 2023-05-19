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
	<AppHeader />

	<main>
		<AppProducts />
	</main>

	<AppFooter />
</template>

<style lang="scss">
@use './assets/styles/general.scss' as *;
// non ho bisogno di reimportare _variables.scss per usare $bg-color perchè in general.scss è stato importato usando @forward
// body {
// 	background-color: $bg-color;
// }
</style>
