<template>
  <div id="app">
	<Cuadro/>
  </div>
</template>

<script>
import Cuadro from './components/Cuadro.vue'
export default {
  name: "App",
  components: {Cuadro},
};

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
