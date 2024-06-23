<script>
	export default {
		name: "Button",
		props: {
			url: String,
			cta: String
		}
	}
</script>

<template>
	<router-link class="btn-1" :to="url">
		{{ cta }}
	</router-link>
</template>

<style scoped>
	.btn-1 {
		display: block;
		width: fit-content;
		
		color: #FFF;
		font-size: 14px;
		text-align: center;

		background: var(--cor-secundaria);
		border: 2px solid transparent;

		padding: 5px 8px;
		border-radius: 20px;

		transition: all .2s ease-in-out;

	}

	.btn-1:hover {
		background: transparent;
		border: 2px solid var(--cor-secundaria);
		transition: all .2s ease-in-out;
	}
</style>