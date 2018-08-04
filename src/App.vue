<template>
  <div id="app">
    <h1>{{ message }}</h1>
    <input v-model="message"/>
    <br/>
    <a :href="url">Click me</a>

    <p v-if="show">Show me</p>
    <p v-else="show">This is else</p>

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'app',
  data() {
    return {
      message: "Hello world from VO4",
      url: 'http://www.cnn.com',
      show: false
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
