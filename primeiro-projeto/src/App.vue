<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <ClubesFutebol />
  </div>
</template>

<script>
import ClubesFutebol from './components/ClubesFutebol.vue'

export default {
  name: 'App',
  components: {
    ClubesFutebol
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
