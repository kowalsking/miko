<template>
  <div class="wraper">
    <Input
      msg="Width"
      type="number"
      :value="width"
    />
    <Input
      msg="Height"
      type="number"
      :value="height"
    />
    <Input
      msg="Background"
      type="color"
      :value="fill"
    />
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'
import Input from './Input.vue'
import { CanvasControlls, InputTypes } from '../enums/enums'

export default Vue.extend({
  components: {
    Input
  },
  props: {
    width: {
      type: Number,
      required: true
    },
    height: {
      type: Number,
      required: true
    },
    fill: {
      type: String,
      required: false,
      default: '#000'
    }
  }
})
</script>

<style scoped>
  .wraper {
    width: 300px;
  }
</style>
