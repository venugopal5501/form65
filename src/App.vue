<template>
  <!-- <img alt="Digital logo" width="300" height="80" src="./assets/Digital_Logo.png"> -->
  <HomePage />
</template>
<script>
import HomePage from './components/HelloWorld.vue'
export default {
  name: 'App',
  components: {
    HomePage
  }
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>