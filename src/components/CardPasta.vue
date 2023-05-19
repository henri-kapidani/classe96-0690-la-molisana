<script>
export default {
	// props: ['urlImg', 'titolo', 'cottura'],
	props: {
		urlImg: String,
		titolo: String,
		cottura: Number,
	},
	// props: {
	// 	urlImg: {
	// 		type: String,
	// 		required: false,
	// 		default: 'indirizzo immagine di default',
	// 	},
	// 	titolo: {
	// 		type: String,
	// 		required: true,
	// 	},
	// 	cottura: {
	// 		type: Number,
	// 		required: false,
	// 	},
	// },
};
</script>

<template>
	<div class="card">
		<img :src="urlImg" :alt="titolo" />
		<h2>{{ titolo }}</h2>
	</div>
</template>

<style lang="scss" scoped>
.card {
	max-width: 25%;
	text-align: center;
	background-color: white;
	border: 2px solid salmon;
}

img {
	width: 100%;
}
</style>
