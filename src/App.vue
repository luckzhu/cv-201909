<template>
  <div id="app">
    <sidebar id="siderbar"></sidebar>
    <div id="main">
      <mainHeader></mainHeader>
    </div>
  </div>
</template>

<script>
import sidebar from "./components/sidebar.vue";
import mainHeader from "./components/main-header.vue";

export default {
  name: "app",
  components: {
    sidebar,
    mainHeader
  }
};
</script>

<style lang="scss">
#app {
  display: flex;
  margin: 0 auto;
  width: 60%;
  padding: 2vw;
  > #siderbar {
    width: 31vw;
    border: 1px solid red;
    background: #e6e7e8;
  }
  > #main {
    width: 67vw;
    border: 1px solid green;
  }
}
</style>
