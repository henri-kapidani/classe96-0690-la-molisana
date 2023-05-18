<script>
export default {};
</script>

<template>
	<header>
		<div class="contents">
			<h2>sono l'<span>header</span></h2>
			<p>
				Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt
				minus quae neque sequi illo excepturi ea recusandae, nostrum optio
				nobis esse rem quasi illum. Quo dicta officiis odit vitae id!
			</p>
		</div>
		<div class="other">
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Obcaecati,
				nostrum quia ducimus vero dolorem perspiciatis, id expedita
				reprehenderit architecto distinctio dicta culpa repellat ab.
				<span>ciao a tutti</span> ab maiores harum modi amet.
			</p>
		</div>
	</header>
</template>

<style lang="scss" scoped>
@use './../assets/styles/partials/variables' as *;
.contents {
	h2 {
		@include my-text-format;
		color: $title-color;

		span {
			color: salmon;
		}

		&:hover,
		&:hover span {
			cursor: pointer;
			text-decoration: underline;
			color: blue;
		}
	}

	p {
		@include my-text-format;
		background-color: yellow;
	}
}
</style>
