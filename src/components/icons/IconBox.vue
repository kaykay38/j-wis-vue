<template>
  <img class="box" src="@/assets/box.svg" :width="width" @click="handleClick" />
</template>
<script lang="ts">
export default {
  props: {
    width: {
      type: String,
      default: '25'
    },
    handleClick: {
      type: Function,
      required: false
    }
  }
}
</script>
<style>
.box {
  display: block;
  margin: 0 auto 1rem;
}
</style>
