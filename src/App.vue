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
    <!-- <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->

    <Footer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import HelloWorld from './components/HelloWorld.vue';
import Story from './components/Story.vue';
import Footer from './components/Footer.vue';

@Component({
  components: {
    Story,
    Footer,
    // HelloWorld,
  },
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
