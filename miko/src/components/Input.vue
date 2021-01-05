<template>
  <div class='wrap'>
    <span>{{ msg }}</span>
    <input
      :type="type"
    />
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'

export default Vue.extend({
  props: {
    type: {
      type: String,
      required: true
    },
    msg: {
      type: String,
      required: true
    }
  }
})
</script>

<style scoped>
  .wrap {
    display: flex;
    justify-content: space-between;
  }

  span {
    margin-right: 20px;
  }

  input {
    width: 40px;
  }
</style>
