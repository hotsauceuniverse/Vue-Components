<template>
<div :class="{ large }" :style="{ backgroundColor: color }" class="btn">{{ text }}</div>
</template>

<script>

export default {
  props: {
    color: {
      type: String,
      default: 'gray'
    },

    large: {
      type: Boolean,
      default: false
    },

    text: {
      type: String,
      default: ''
    }
  }
}
</script>



<style scoped>
  .btn {
    display: inline-block;
    margin: 4px;
    padding: 6px 12px;
    border-radius: 4px;
    background-color: gray;
    color: white;
    cursor: pointer;
  }

  .btn.large {
    font-size: 20px;
    padding: 10px 20px;
  }
</style>
