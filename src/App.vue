<template>
  <div id="app">
      <index></index>
    
  </div>
</template>

<script>
import "./stylesheets/reset.css"
import "../static/font/iconfont.css"
import Index from "./components/Index"

export default {
  name: 'App',
  components:{
    Index
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  /* width:100%;
  height:100%; */
}
</style>
