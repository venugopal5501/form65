<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HomePage msg="Welcome to Your Vue.js App"/>
   <HomePage/>
  <userPage item="some data" name="user-cmp"/>
  <computeProperty/>
  <yesNo/>
</template>

<script>
import HomePage from './components/HelloWorld.vue'
import userPage from './components/User.vue'
import computeProperty from './components/template_expression.vue'
import yesNo from './components/computed.vue'

export default {
  name: 'App',
  components: {
    HomePage,
    userPage,
    computeProperty,
    yesNo
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
