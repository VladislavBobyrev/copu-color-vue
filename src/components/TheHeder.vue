<template>
  <header>
    <img width="32" height="32" alt="Vue logo" src="../assets/logo.png">
    <h1>Your like color</h1>
  </header>
</template>

<script>
export default {
data(){
  return{
    color: '#fff000'
  }
}
}
</script>

<style lang="scss" scoped>
  header{
    display: flex;
    align-items: center;
    justify-content: space-around;
    background: rgb(183, 188, 89);
  }
</style>

