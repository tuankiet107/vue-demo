<template>
  <div id="app">
    <router-link :to="{ name: 'home' }">Home</router-link>
    <router-link to="/profiles">Profiles</router-link>
    <!-- <router-link to="/profiles/:id"></router-link> -->
    <router-view></router-view>
  </div>
</template>

<script>

export default {
  name: "App",
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
a{
  margin: 0 10px;
}
</style>
