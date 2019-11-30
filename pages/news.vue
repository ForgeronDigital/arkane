<template>
  <div>
    <Header />
    <NewCardDetail />
  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue'
import Header from "@/components/Header.vue";
import NewCardDetail from "@/components/NewCardDetail.vue";

export default {
  components: {
    // Logo
    Header,
    NewCardDetail
  }
};
</script>

<style>
</style>
