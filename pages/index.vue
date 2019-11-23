<template>
  <div>
    <Header />
    <News />
  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue'
import Header from "@/components/Header.vue";
import News from "@/components/News.vue";

export default {
  components: {
    // Logo
    Header,
    News
  }
};
</script>

<style>
</style>
