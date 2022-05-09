<template>
  <main>
    <section>
      <div class="jumbotron"></div>
    </section>
    <section>
      <div class="container">
        <h2>Current Series</h2>
        <ComicsTron />
        <button>Load More</button>
      </div>
    </section>
  </main>
</template>

<script>
import ComicsTron from "./sections/ComicsTron.vue";

export default {
  name: "MainTron",
  components: {
    ComicsTron,
  },
};
</script>

<style scoped lang="scss">
main {
  background-color: #1c1c1c;
  color: white;
}

.jumbotron {
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: cover;
  height: 265px;
}

section:last-of-type {
  font-family: "Bangers", cursive;
}

.container {
  font-family: "Bangers", cursive;
  flex-direction: column;
  align-items: flex-start;

  padding-bottom: 20px;

  h2 {
    font-size: 40px;
    background-color: #0282f9;
    padding: 10px 30px;

    transform: translate(0, -50%);
  }

  button {
    font-family: "Bangers", cursive;
    font-size: 16px;
    padding: 10px 70px;
    align-self: center;
    background-color: #0282f9;
  }
}
</style>
