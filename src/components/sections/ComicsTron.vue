<template>
  <div class="series-container">
    <Comic v-for="(element, i) in comics" :key="i" :comic="element" />
  </div>
</template>

<script>
import Comic from "./Comic.vue";
import comicsData from "../../data/dc-comics.json";

export default {
  name: "CosmicTron",
  components: {
    Comic,
  },
  data() {
    return {
      comics: comicsData,
    };
  },
};
</script>

<style scoped lang="scss">
.series-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
