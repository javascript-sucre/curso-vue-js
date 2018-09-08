<template>
  <div id="app">
    <Menu/>
    <Header/>
    <Search/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Menu from './components/Menu.vue';
import Search from './components/Search.vue';

export default {
  name: 'app',
  components: {
    Header,
    Menu,
    Search
  }
}
</script>

<style>
body{
  background-color: #08132f;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
}
</style>
