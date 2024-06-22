<script>
	import Button from '../../Global/Button.vue'
	export default {
		name: "About",
		components: {
			Button
		}
	}
</script>

<template>
	<main class="section about">
		<section class="about-cta">
			<div class="headline">
				<h2 class="title">
					Crie seu império digital com a CIER
				</h2>
				<p class="subtitle-orbitron">Seja a próxima grande história de sucesso.</p>
			</div>

			<p class="text">Você está pronto para levar seu negócio para o próximo nível?
			A <span class="text-highlight">CIER</span> é o seu parceiro ideal. Nós fornecemos serviços digitais para te ajudar a alcançar novos patamares:
			</p>

			<ul class="services">
				<li class="services-item text">
					desenvolvimento web
				</li>

				<li class="services-item text">
					Copywriting
				</li>

				<li class="services-item text">
					marketing digital
				</li>

				<li class="services-item text">
					social media
				</li>
			</ul>

			<p class="text">vamos te ajudar a construir uma marca forte e uma presença online impactante.</p>

			<Button cta="Ver todos os serviços"/>
		</section>

		<img class="image" src="../../../assets/images/vetores/goals.png">
	</main>
</template>

<style scoped>
	.about {
		background-color: var(--fundo-azul);
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.subtitle-orbitron {
    	color: var(--cor-principal);
	}

	.about-cta {
		display: flex;
		flex-direction: column;
		justify-content: left;

		gap: 33px;

		width: 50%;
	}

	.text {
		text-transform: uppercase;
	}

	.services {
		list-style: inside;

		display: flex;
		flex-direction: column;
		gap: 6px;
	}

	.services-item {
		color: var(--cor-principal);
	}

	.image {
		width: 40%;
		image-rendering: optimizeSpeed;
	}
</style>