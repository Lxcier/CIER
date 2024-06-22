<script>
	import Navbar from './Navbar.vue'
	import Logo from './Logo.vue'
	import Button from './Button.vue'

	export default {
		name: "Header",
		components: {
			Navbar, 
			Logo,
			Button
		}
	}
</script>

<template>
	<header class="header">
		<Navbar/>
		<Logo/>
		<Button url="#" cta="Fazer Orçamento"/>
	</header>
</template>

<style scoped>
	header.header {
		max-width: 1440px;
		width: 100%;
		margin: 0 auto;
		padding: 17px 60px;
		
		display: flex;
		align-items: center;
		justify-content: space-between;

		position: sticky;
		top: 0;
		left: 0;
	}
</style>