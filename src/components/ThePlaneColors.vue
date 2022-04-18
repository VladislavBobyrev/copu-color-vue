<template>
   <section class="plane-colors" v-bind:style="{background :updateColrs}">
     
      <input
      @click="getVal"
       type="text" id="input-colors" placeholder="Your colors" 
       :value="updateColrs">
      <label for="input-colors"><h2>Click me for copy colors</h2></label>
    </section>
</template>

<script>
export default {
  props: ['updateColrs'],
  data() {
    return
    {
      text: String
    }
  },
methods: {
  getVal(e) { 
    navigator.clipboard.writeText(e.target.value)
    .then(() => {
      alert(`SUCSECC copy colors ${e.target.value}`)
    })
  },

}

  }
</script>

<style>
.plane-colors{
width: 100%;
height: 100%;
display: flex;
justify-content: center;
align-items: center;
gap: 8px;
  background: rgb(229, 169, 169);
}
</style>