<template>
  <div class="newContainer bkg-dark mb10">
    <div class="flex space-between title-card-container">
      <h3 class="card-title">{{title}}</h3>
      <p class="card-date">{{date}}</p>
    </div>
    <h4 class="mb10">{{subtitle}}</h4>
    <p class="card-content color-dark">{{content}}</p>
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
    content: String,
    id: String
  }
};
</script>

<style scoped>
.newContainer {
  height: 100%;
  width: calc(100% - 80px);
  color: white;
  margin: 40px;
  padding: 10px;
}
.title-card-container {
  width: 100%;
}
.card-title {
  /* margin-left: 10px; */
}
.card-date {
  /* margin-right: 10px; */
}
.card-content {
  width: 100%;
  height: 75%;
  background-color: white;
  padding: 5px;
}
</style>