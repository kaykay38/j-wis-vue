<template>
  <img class="logo" src="@/assets/logo.svg" @click="handleClick" />
</template>
<script lang="ts">
export default {
  props: {
    width: {
      type: String,
      default: '125'
    },
    handleClick: {
      type: Function,
      required: false
    }
  }
}
</script>
<style>
.logo {
  display: block;
  margin: 0 auto 2rem;
}
</style>
