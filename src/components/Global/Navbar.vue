<script>
	export default {
		name: "Navbar",
		data(){
			return {
				isActive: true,
				navbar: {
					item: [
						{
							id: 1,
							option: "Sobre",
							url: "#"
						},
						{
							id: 2,
							option: "Serviços",
							url: "#"
						},
						{
							id: 3,
							option: "Projetos",
							url: "#"
						}

						]
					}
				} 
		}
	}
</script>

<template>
	<ul class="navbar">
		<li class="navbar__item text" v-for="item in navbar.item">
			<a @click="e => e.target.classList.toggle('link-isActive')":href="item.url">
				{{item.option}}
			</a>
		</li>
	</ul>
</template>

<style scoped>
	ul.navbar {
		display: flex; 
		align-items: center;
		gap: 1.6rem;
		text-align: center;
		list-style: none;
	}

	
	ul.navbar > li.navbar__item a{
		color: var(--cor-principal);
		transition: all .3s ease-in-out;
	}

	ul.navbar > li.navbar__item a:hover{
		color: var(--branco);
		transition: all .3s ease-in-out;

	}

	ul.navbar > li.navbar__item a.link-isActive{
		color: var(--branco);
	}

</style>