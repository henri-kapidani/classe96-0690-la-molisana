<script>
export default {
	data() {
		return {
			menuData: [
				{
					name: 'Home',
					src: '#',
					active: false,
				},
				{
					name: 'Prodotti',
					src: '#',
					active: false,
				},
				{
					name: 'Chi siamo',
					src: '#',
					active: false,
				},
				{
					name: 'Contatti',
					src: '#',
					active: false,
				},
			],
		};
	},
};
</script>

<template>
	<nav>
		<ul>
			<li v-for="menuItem in menuData" :key="menuItem.name">
				<a :href="menuItem.src">{{ menuItem.name }}</a>
			</li>
		</ul>
	</nav>
</template>

<style lang="scss" scoped>
ul {
	display: flex;
	justify-content: center;
	gap: 0.5rem;
	list-style: none;
}
</style>
