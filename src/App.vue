<template>
  <div id="app">
    <Index />
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Header from './components/Header.vue'
import Index from './components/Index.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Header,
    Index
  }
}
</script>

<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50; */
  /* margin-top: 60px; */
}

.color-grey {
  color: #dddfd4
}

.color-yellow {
  color: #fae598;
}

.color-lightblue{
  color: #3fb0ac
}

.color-darkblue{
  color: #173e43
}
</style>
