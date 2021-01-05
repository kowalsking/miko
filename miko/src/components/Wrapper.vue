<template>
  <div>
    <Canvas
      :width="width"
      :height="height"
      :fill="fill"
    />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Canvas from './Canvas.vue'

export default Vue.extend({
  components: {
    Canvas
  },
  data: () => ({
    width: 600,
    height: 800,
    fill: 'cyan'
  })
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
