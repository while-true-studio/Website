<template>
	<div id="app">
		<section class="hero is-dark is-large is-bold">
			<div class="hero-body">
				<div class="container">
					<img alt="Vue logo" src="./assets/goblinslayer.png">
					<h2 class="subtitle">
						Un juego hack'n'slash donde te enfrentarás a muchos goblins, ¿te atreves?
					</h2>
				</div>
			</div>
		</section>

		<Story />
		<Downloads />

		<h1 class="title">Equipo</h1>
		<TeamMember imageSRC="Members/Stiven.jpg" name="Stiven Arias"
			description="Amante de la filosofía y de la buena compañía. Friki incondicional y emprendedor de sueños locos."/>
		<TeamMember imageSRC="Members/Oscar.jpg" name="Óscar Fernández"
			description="Un diseñador en proceso (con espíritu de ingeniero). Aparte me gusta el Freestyle. De todo tipo. Dame un palo de golf por ejemplo y me hago un mortal."/>
		<TeamMember imageSRC="Members/Borja.jpg" name="Borja Cano"
			description="TBD."/>
		<TeamMember imageSRC="Members/Antonio.jpg" name="Antonio Román"
			description="Amante de la música y de la programación, literalmente hice un proyecto de 3 meses en 3 días."/>
		<TeamMember imageSRC="Members/Anass.jpg" name="Anass Carreau"
			description="Apasionado  por la música el deporte y los videojuegos. Me gusta ayudar a las personas aunque no sepa ni ayudarme. Traigo el disco duro en vez de subirlo al Git."/>
		<Footer />
	</div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import HelloWorld from './components/HelloWorld.vue';
import Story from './components/Story.vue';
import Downloads from './components/Downloads.vue';
import Footer from './components/Footer.vue';
import TeamMember from './components/TeamMember.vue';

@Component({
	components: {
		Story,
		Downloads,
		TeamMember,
		Footer,
		// HelloWorld,
	}
})
export default class App extends Vue {}
</script>

<style lang="scss">
@import "~bulma/sass/utilities/initial-variables";
$footer-background-color: $grey-darker;

@import "~bulma/sass/layout/footer";

a {
	color: $blue;
}

a:hover {
	color: $cyan;
}
</style>

<style>
#app {
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 0px;
}
</style>
