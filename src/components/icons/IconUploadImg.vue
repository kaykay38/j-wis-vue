<template>
  <img src="@/assets/upload.svg" @click="handleClick" />
</template>
<script lang="ts">
export default {
  props: {
    width: {
      type: String,
      default: '100%',
      required: false
    },
    handleClick: {
      type: Function,
      required: false
    }
  }
}
</script>
<style></style>
