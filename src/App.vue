<template>
  <div id="app">
 <h1>hola</h1>
  <ListaDeTareas> </ListaDeTareas>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import ListaDeTareas from './components/ListaDeTareas.vue'

export default {
  name: 'App',
  components: {
    ListaDeTareas
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
