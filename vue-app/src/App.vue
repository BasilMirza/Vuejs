<template>
  <div id="app">
    <Example/>
    <ClickCounter/>
    <HoverCounter/>
  </div>
</template>

<script>
import Example from './components/Example.vue'
import ClickCounter from './components/ClickCounter'
import HoverCounter from './components/HoverCounter'

export default {
  name: 'App',
  components: {
    Example,
    ClickCounter,
    HoverCounter,
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
