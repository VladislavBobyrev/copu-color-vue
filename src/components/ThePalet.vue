<template>
      <section class="pick-colors">
      <h2>Select colors</h2>
        {{paletColors}}
      <input v-model="paletColors"
       type="color"  id="palet"
       @input="getColors"> 
    </section>
</template>

<script>
export default {
emits: ['paletColors'],
methods: {
  getColors() {
    this.$emit('getColors', {
      color: this.paletColors
      })
  }
}
}
</script>
