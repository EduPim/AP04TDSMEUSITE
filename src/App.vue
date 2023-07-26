<template>
  <div id="app">
    <h1>CatS Editor</h1>
    <Cat></Cat>
  </div>
</template>

<script>
import Cat from './components/Cat'

export default {
  name: 'App',
  components: {
    Cat
  }
}
</script>


<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2b2b2b;
  margin-top: 60px;
  background-image: url('assets/CAIXAS.jpg');
  background-size: 100%;
}

</style>
