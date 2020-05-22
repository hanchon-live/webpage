<template>
  <div id="app">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700;900&amp;display=swap" rel="stylesheet">
    <IndexHorizontal />
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Header from './components/Header.vue'
// import Index from './components/Index.vue'
import IndexHorizontal from './components/IndexHorizontal.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Header,
    // Index,
    IndexHorizontal
  }
}
</script>

<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;*/
  color: #2c3e50; 
  /* margin-top: 60px; */
}
@-ms-viewport {
		width: device-width;
}

body {
  -ms-overflow-style: scrollbar;
  font-family: "Poppins", sans-serif;
  background: #f1f3f5;
  widows: 100%;
  width: 100%;
  /* overflow: hidden; */
}

@media screen and (max-width: 360px) {

  html, body {
    min-width: 320px;
  }

}

html {
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: inherit;
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
