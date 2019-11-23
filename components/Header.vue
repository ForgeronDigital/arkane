<template>
  <div class="flex align-center column header-container mb10 bkg-dark">
    <nuxt-link to="/">
      <img src="../assets/img/logo.png" alt="logo-arkane" class="logo" />
    </nuxt-link>
    <h1 class="gold mb10">Arkane, courtier et gestionnaire de patrimoine</h1>
    <Navbar />
  </div>
</template>
<script>
import Navbar from "./Navbar.vue";
export default {
  components: {
    // Logo
    Navbar
  }
};
</script>

<style scoped>
.logo {
  height: 200px;
  width: 200px;
}
.header-container {
  width: 100vw;
  padding-top: 30px;
}
</style>