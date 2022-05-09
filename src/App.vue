<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style lang="scss">
#app {
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  li {
    list-style: none;
  }

  a {
    text-decoration: none;
  }

  .container {
    max-width: 1280px;
    margin: auto;
    display: flex;
    align-items: center;
  }

  button {
    background: none;
    border: 2px solid #0282f9;
    color: white;
    cursor: pointer;
    &:hover {
      background-color: #0282f9;
    }
  }
}
</style>
