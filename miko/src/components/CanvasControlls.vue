<template>
  <div class="wraper">
    <Input
      msg="Width"
      type="number"
    />
    <Input
      msg="Height"
      type="number"
    />
    <Input
      msg="Background"
      type="color"
    />
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'
import Input from './Input.vue'

export default Vue.extend({
  components: {
    Input
  }
})
</script>

<style scoped>
  .wraper {
    width: 300px;
  }
</style>
