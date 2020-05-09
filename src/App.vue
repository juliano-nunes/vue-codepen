<template>
  <div id="app">
    <h1>Codepen</h1>
    <textarea cols="100" rows="20" v-model="insecureHTML" placeholder="Escreva seu texto em html"></textarea>

    <h2>Result:</h2>
    <div v-html="insecureHTML"></div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      insecureHTML: ''
    }
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
