<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Malena no se baña y Raiza TARU"/>
  <SaludosTodos></SaludosTodos>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SaludosTodos from './components/SaludosTodos.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    SaludosTodos
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0643a041;
  margin-top: 60px;
}
</style>
