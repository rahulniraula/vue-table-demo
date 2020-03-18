<template>
  <div id="app">
    <country-list/>
  </div>
</template>

<script>
import countryList from "./components/country-list";

export default {
  name: 'App',
  components: {
    countryList
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
