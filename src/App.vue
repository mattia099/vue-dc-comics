<template>
  <div id="app">
    <appHeader />
    <appMain />
    <appFooter />
  </div>
</template>

<script>
import appHeader from './components/appHeader.vue'
import appMain from './components/appMain.vue'
import appFooter from './components/appFooter.vue'

export default {
  name: 'App',
  components: {
    appHeader,
    appMain,
    appFooter
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  max-width: 1280px;
  margin: 0 auto;
}

</style>
