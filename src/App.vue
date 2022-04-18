<template>
  <TheHeader/>
  <TheMain/>
</template>

<script>
import TheHeader from './components/TheHeder.vue'
import TheMain from './components/TheMain.vue' 

export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain
  }
}
</script>

<style lang="scss">
body, html{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  width: 100vw;
  height: 100vh;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow: hidden;
  height: 100%;
display: grid;
grid-template: 50px 1fr/ auto;
}
</style>
