<template>
  <div id="app">
    <topBar/>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <CreatedComponent/>
    <bottomBar/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import CreatedComponent from './components/CreatedComponent.vue';
import topBar from './components/topBar.vue';
import bottomBar from './components/bottomBar.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    CreatedComponent,
    topBar,
    bottomBar,
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
