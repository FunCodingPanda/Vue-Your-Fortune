<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/d20.png">
    <Random msg="Your Fate Will Be Determined By the Die"/>
  </div>
</template>

<script>
import Random from './components/Random.vue'

export default {
  name: 'app',
  components: {
    Random
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
