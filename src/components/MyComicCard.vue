<template>
  <div class="comic">
    <div class="comic__img-container">
      <img :src="comicObj.thumb" :alt="comicObj.series" />
    </div>
    <h4>{{ comicObj.series }}</h4>
  </div>
</template>

<script>
export default {
  name: "MyComicCard",
  props: {
    comicObj: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/commons.scss";

.comic {
  width: calc(100% / 6);
  margin-top: 2rem;

  &__img-container {
    width: 200px;
    height: 200px;
    overflow: hidden;
  }

  h4 {
    text-transform: uppercase;
    color: white;
    margin: 1rem 0;
    font-weight: 500;
  }
}
</style>
