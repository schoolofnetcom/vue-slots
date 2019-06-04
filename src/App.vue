<template>
  <div id="app">
    <layout>
      <template v-slot:footer>
        <p>Ir para o site da School of  Net</p>
      </template>

      <template v-slot:header>
        <img src="./assets/logo.png">
      </template>

      <e-btn href="https://schoolofnet.com" target="_blank">
        <i class="material-icons">school</i>
        {{ name }}
      </e-btn>
    </layout>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import EBtn from './components/button'
import layout from './components/layout'

export default {
  name: 'App',
  data() {
    return {
      name: 'School of Net',
    };
  },
  components: {
    HelloWorld,
    'e-btn': EBtn,
    layout
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
