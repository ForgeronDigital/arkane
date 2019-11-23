<template>
  <div class="newContainer bkg-dark">
    <div class="flex space-between">
      <h3>{{title}}</h3>
      <p>{{date}}</p>
    </div>
    <h4>{{subtitle}}</h4>
    <p>{{content}}</p>
  </div>
</template>
<script>
// import Navbar from "./Navbar.vue"
export default {
  components: {},
  props: {
    title: String,
    date: String,
    subtitle: String,
    content: String
  }
};
</script>

<style scoped>
.newContainer {
  height: 250px;
  width: 250px;
  color: white;
  margin: 20px;
}
</style>