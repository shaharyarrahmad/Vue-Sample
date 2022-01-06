<template>
  <div>
    <HeaderVue />
    <Nuxt />
    <FooterVue />
  </div>
</template>
<script>
import HeaderVue from "../components/layout/header.vue"
import FooterVue from "../components/layout/stickyRegister.vue"
export default {
  components: {
    HeaderVue,
    FooterVue
  },
}
</script>
<style scoped>
#app {
  font-family: 'Lato', sans-serif;
  background: transparent linear-gradient(141deg, #EBF4FF 0%, #E6FFFA 100%) 0% 0% no-repeat padding-box;
}

</style>
