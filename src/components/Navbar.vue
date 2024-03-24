<template>
  <nav class="navbar">
    <IconJWis :handleClick="handleLogoClick" class="logo" />
  </nav>
</template>

<script lang="ts">
import IconJWis from '@/components/icons/IconJWis.vue'
export default {
  name: 'NavBar',
  methods: {
    handleLogoClick() {
      console.log('Logo clicked')
      this.$router.push('/')
    }
  },
  components: {
    IconJWis
  }
}
</script>

<style scoped>
.navbar {
  background-color: #fff;
  color: #333;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: auto;
  min-width: 100vw;
  height: 72px;
  margin: 0px;
}

.logo {
  height: 33px;
  width: auto; /* Let the logo adjust its width based on its aspect ratio */
  cursor: pointer;
  padding: 0px;
  margin: 0px;
}
</style>
