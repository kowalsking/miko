<template>
  <div>
    <Canvas />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Canvas from './Canvas.vue'

export default Vue.extend({
  components: {
    Canvas
  }
})
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
