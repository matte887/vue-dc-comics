<template>
  <div id="app">
    <div class="container">
      <MyHeader />
      <main>
        <h2>--> Content goes here <--</h2>
      </main>
    </div>
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";

export default {
  name: "App",
  components: {
    MyHeader,
  },
};
</script>

<style lang="scss">
@import "./style/commons.scss";
@import "./style/variables.scss";

.container {
  width: 70%;
  margin: 0 auto;
}

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
