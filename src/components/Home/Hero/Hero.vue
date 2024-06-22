<script>
	import Button from '../../Global/Button.vue'
	export default {
		name: "Hero",
		components: {
			Button
		}
	}

</script>

<template>
	<main class="section hero">
		<section class="hero-cta">
			<h1 class="title-big" >O <span class="text-highlight">Mundo Digital</span> ao Seu Alcance.</h1>

			<p class="subtitle-orbitron">Já imaginou transformar completamente o seu negócio com a ajuda da internet?</p>

			<Button cta="Quero saber mais"/>
		</section>

		<p class="hero-text subtitle-orbitron"w>Uma pesquisa feita pela HostGator mostrou que 58% das empresas aumentaram o investimento digital na pandemia, com 64% tendo <span class="text-highlight">aumento nas vendas</span>.</p>
	</main>
</template>

<style scoped>
	.hero {
		background: url('../../../assets/images/banners/hero-banner.png');
		background-repeat: no-repeat;
		background-size: cover;
		margin-top: -82px;
		height: 650px;

		display: flex;
		align-items: center;
		justify-content: space-between;

		gap: 20px;
	}

	.hero-cta {
		text-align: left;

		display: flex;
		flex-direction: column;

		max-width: 48%;

		& h1 {
			margin-bottom: 26px;
		}

		& .text-highlight {
			font-weight: 500;
		}

		& p {
			margin-bottom: 60px;
		}
	}

	.hero-text {
		width: 34%;
		text-align: right;
	}
</style>