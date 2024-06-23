<script>
	import Button from '../../Global/Button.vue'

	import Glide from './Glide.vue'
	

	export default {
		name: "Services",
		components: {
			Button,
			Glide
		}
	}
</script>

<template>
	<main class="section services">
		<div class="headline">
			<h2 class="title">Serviços digitais personalizados para o seu sucesso</h2>
			<p class="subtitle">Descubra como podemos te ajudar a alcançar os seus objetivos.</p>
		</div>

		<Glide/>
	</main>
</template>

<style scoped>
	.services {
		background: linear-gradient(#111134 0%,  #0D0D21 100%);
	}
	.headline {
		width: fit-content;
		margin: 0 auto;
		text-align: center;
		text-transform: uppercase;
	}


</style>