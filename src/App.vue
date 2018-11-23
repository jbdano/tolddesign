<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to your Vue.js App"/> -->
    <home-hero />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import HomeHero from './components/HomeHero.vue';

export default {
  name: 'app',
  components: {
    HomeHero,
  },
};
</script>

<style lang="scss">

html, body {
  overflow-x: hidden;
}

body {
  margin: 0px !important;
}

.theme-color-green {
  color: #50ada2;
}

.theme-color-white {
  color: #FCFAF9;
}

.theme-inline-button {
  display: inline-block;
  padding: 20px;
  text-decoration: none;
  border-radius: 5px;
  border: 3px solid #50ada2;
  font-size: 14px;
  transition: all 0.3s ease-out;

  &:hover {
    background-color: #50ada2;
    color: #FCFAF9;
  }
  &:focus {
    outline: 0;
  }
}

.theme-inline-button-primary {
  background-color: #50ada2;
  color: #FCFAF9;
}

.theme-inline-button-secondary {
  background-color: transparent;
  color: #50ada2;
}

h1, h2, h3, h4, h5, p, a {
  font-family: 'Josefin Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
}

h1 {
  font-size: calc(46px + (80 - 46) * ((100vw - 300px) / (1600 - 300)));
  margin: 0;
}

p, a {
  font-size: calc(14px + (24 - 14) * ((100vw - 300px) / (1600 - 300)));
}

</style>
