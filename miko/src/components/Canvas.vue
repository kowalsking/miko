<template>
  <div>
    <canvas
      id="miko"
      :width="width"
      :height="height"
    ></canvas>
    <CanvasControlls />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import CanvasControlls from './CanvasControlls.vue'

export default Vue.extend({
  components: {
    CanvasControlls
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
  },
  mounted () {
    const canvas: HTMLCanvasElement = document.querySelector('#miko')
    const ctx: CanvasRenderingContext2D = canvas.getContext('2d')
    ctx.fillStyle = this.$props.fill
    ctx.fillRect(0, 0, this.$props.width, this.$props.height)
  }
})
</script>

<style>

</style>
