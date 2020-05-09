<template>
  <div id="app">
    <h1>Codepen</h1>
    <textarea cols="100" rows="20" v-model="insecureHTML" placeholder="Write down your html here"></textarea>

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
  body {
    background-color: black;
  }
  textarea {
    background-color: cadetblue;
    border: solid 2px darkturquoise;
    font-size: 1.5rem;
  }
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: darkturquoise;
    margin-top: 60px;
  }
</style>
