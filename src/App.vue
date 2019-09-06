<template>
  <div id="app">
    <sidebar id="siderbar"></sidebar>
    <div id="main">
      <mainHeader></mainHeader>
      <education></education>
      <project class="project"></project>
      <personal></personal>
    </div>
    
  </div>
</template>

<script>
import sidebar from "./components/sidebar.vue";
import mainHeader from "./components/main-header.vue";
import education from "./components/education.vue";
import project from "./components/project.vue";
import personal from "./components/personal.vue";
export default {
  name: "app",
  components: {
    sidebar,
    mainHeader,
    education,
    project,
    personal
  }
};
</script>

<style lang="scss">
#app {
  display: flex;
  margin: 0 auto;

  > #siderbar {
    width: 30vw;

    background: #e6e7e8;
  }
  > #main {
    width: 70vw;
    box-shadow: 0 0 0 1px rgb(225, 225, 225);
    .project {
      margin-top: 2vw;
    }
  }
}
</style>
