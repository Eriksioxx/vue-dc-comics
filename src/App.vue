<template>
  <div id="app">
    <Header />
    <MainTron />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MainTron from "./components/MainTron.vue";

export default {
  name: "App",
  components: {
    Header,
    MainTron,
  },
};
</script>

<style lang="scss">
@import "./assets/styles/global.scss";
</style>
