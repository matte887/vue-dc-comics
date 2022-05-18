<template>
  <div id="app">
    <MyHeader />
    <main>
      <MyComicList />
    </main>
    <MyBlueNav />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyFooter from "./components/MyFooter.vue";
import MyBlueNav from "./components/MyBlueNav.vue";
import MyComicList from "./components/MyComicList.vue";

export default {
  name: "App",
  components: {
    MyHeader,
    MyFooter,
    MyBlueNav,
    MyComicList,
  },
};
</script>

<style lang="scss">
@import "./style/commons.scss";
@import "./style/variables.scss";

main {
  width: 100%;
  background-color: $main-background-color;
  h2 {
    color: white;
    text-align: center;
    line-height: 150px;
  }
}
</style>
