<template>
  <nav class="navbar">
    <img src="@/assets/logo.svg" alt="Logo" @click="goHome" class="logo" />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Navbar',
  methods: {
    handleLogoClick() {
      this.$router.push('/')
    }
  },
  components: {}
})
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
import type IconJWisLogoVue from './icons/IconJWisLogo.vue';import type IconJWisLogoVue from
'@/components/icons/IconJWisLogo.vue';import type IconJWisLogoVue from './icons/IconJWisLogo.vue';
