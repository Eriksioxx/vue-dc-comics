<template>
  <div class="comic">
    <a href="#">
      <div class="comic-thumb">
        <img :src="comic.thumb" :alt="comic - series" />
      </div>
      <div class="comic-series">
        {{ comic.series }}
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: "ComicCentral",
  props: {
    comic: Object,
  },
};
</script>

<style scoped lang="scss">
.comic {
  height: 260px;
  width: 210px;
  padding: 0 10px;

  a {
    color: white;
  }

  .comic-thumb {
    height: 175px;
    text-align: center;
    overflow: hidden;

    img {
      width: 175px;
    }
  }

  .comic-series {
    margin: 15px 7px;
  }
}
</style>
