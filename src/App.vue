<template>
  <div id="app">
    <Header msg="Welcome to Your Vue.js App"/>
    <Hero/>
    <Productos/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import Productos from "./components/Productos.vue";

export default {
  name: "app",
  components: {
    Header,
    Hero,
    Productos
  }
};
</script>

<style>
#app {
  /* font-family: "Avenir", Helvetica, Arial, sans-serif; */
  font-family: "Open Sans", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
