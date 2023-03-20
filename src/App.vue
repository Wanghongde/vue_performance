<template>
  <div id="app">
    <!-- <Freeze /> -->

    <!-- <AllFunc /> -->

    <NorRen />
  </div>
</template>

<script>
// import Freeze from './components/01-Freeze.vue'

// import AllFunc from './components/02-allCom.vue'

// import NorRen from './components/03-normalRender.vue'
import NorRen from './components/03-delayRender.vue'

export default {
  name: 'App',
  components: {
    // Freeze,

    // AllFunc,

    NorRen
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
