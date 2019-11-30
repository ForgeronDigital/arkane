<template>
  <div class="navbar-container flex space-around shadow">
    <nuxt-link to="/" class="text-dec-none bold color-dark">Accueil</nuxt-link>
    <nuxt-link to="quiSommesNous" class="text-dec-none bold color-dark">Qui sommes nous ?</nuxt-link>
    <nuxt-link to="/courtage" class="text-dec-none bold color-dark">Courtage</nuxt-link>
    <nuxt-link
      to="/gestion-de-patrimoine"
      class="text-dec-none bold color-dark"
    >Gestion de patrimoine</nuxt-link>
    <nuxt-link
      to="espaceClient"
      class="text-dec-none bold color-dark"
      v-if="connected"
    >Espace client</nuxt-link>
    <div class="connexion flex space-around" v-if="!connected">
      <label for="id" class="connexion-input">
        <input type="text" name="id" id="id" placeholder="Identifiant" />
      </label>
      <label for="psw" class>
        <input type="password" name="psw" id="psw" placeholder="Mot de passe" />
      </label>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      connected: false
    };
  }
};
</script>

<style scoped>
.navbar-container {
  width: 100vw;
  background-color: white;
  padding: 10px;
}
.shadow {
  box-shadow: 0 10px 30px black;
  border-radius: 0;
}
.connexion-input {
  margin-right: 10px;
}
</style>