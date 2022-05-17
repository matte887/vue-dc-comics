<template>
  <div id="app">
    <MyHeader />
    <main>
      <h2>Content goes here</h2>
    </main>
    <MyBlueNav />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyFooter from "./components/MyFooter.vue";
import MyBlueNav from "./components/MyBlueNav.vue";

export default {
  name: "App",
  components: {
    MyHeader,
    MyFooter,
    MyBlueNav,
},
};
</script>

<style lang="scss">
@import "./style/commons.scss";
@import "./style/variables.scss";

main {
  width: 100%;
  height: 150px;
  background-color: $main-background-color;
  h2 {
    color: white;
    text-align: center;
    line-height: 150px;
  }
}
</style>
