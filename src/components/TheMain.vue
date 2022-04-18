<template>
  <main class="main">
   <ThePlaneColors :updateColrs="color"/>
   <ThePalet @getColors='postColors'/>
  </main>
</template>

<script>
import ThePlaneColors from "./ThePlaneColors.vue"
import ThePalet from "./ThePalet.vue"

export default {
  data() {
    return{
      color: '#6778ad'
    }
  }, 
  methods: {
   postColors(data){
     data.color
     this.color = data.color
    }
  },
 components: {
   ThePlaneColors,
   ThePalet
 }
}
</script>

<style lang="scss" scoped>
main{
  display: grid;
  grid-template: 1fr / 1fr 1fr ;
  align-items: center;
  width: 100%;
}
</style>