<template>
  <div class>
    <h2>Actualités :</h2>
    <div class="flex center wrap newsContainer">
      <NewCard
        v-for="(newComponent, index) in news"
        :key="index"
        :title="newComponent.title"
        :date="newComponent.date"
        :subtitle="newComponent.subtitle"
        :content="newComponent.content"
      />
    </div>
  </div>
</template>
<script>
import NewCard from "./NewCard.vue";
export default {
  components: {
    NewCard
  },
  data() {
    return {
      news: require("@/news.json")
    };
  },
  mounted() {
    // console.log(this.$data.news);
  }
};
</script>

<style scoped>
.newsContainer {
  margin: 10px;
}
</style>