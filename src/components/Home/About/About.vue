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
				<h2 class="title autoShow">
					Crie seu império digital com a CIER
				</h2>
				<p class="subtitle">Seja a próxima grande história de sucesso.</p>
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

		<img class="image autoScale" src="../../../assets/images/vetores/goals.png">
	</main>
</template>

<style scoped>
	.about {
		background: linear-gradient(#1D1D3F 35%, #111134 100%);
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.headline .title{
		margin: 0;
		padding: 0;
	}

	.about-cta {
		display: flex;
		flex-direction: column;
		justify-content: left;

		gap: 3.3rem;

		width: 50%;
	}

	.text {
		text-transform: uppercase;
	}

	.services {
		list-style: inside;

		display: flex;
		flex-direction: column;
		gap: .6rem;
	}

	.services-item {
		color: var(--cor-principal);
	}

	.image {
		width: 40%;
		image-rendering: optimizeSpeed;
	}

	.autoScale {
		animation: autoScaleAnimation;
		animation-duration: 1.5s;
	}

	@keyframes autoScaleAnimation {
		from {
			transform: scale(0);
		}
		to {
			transform: scale(1);
		}
	}

	.autoShow {
		animation: autoShowAnimation;
		animation-timeline: view(40% auto);
	}

	@keyframes autoShowAnimation {
		from {
			opacity: 0;
			transform: translateY(200px) scale(0.3);
		}to{
			opacity: 1;
			transform: translateY(0) scale(1);
		}
	}
</style>