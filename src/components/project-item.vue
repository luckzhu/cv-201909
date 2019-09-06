<template>
  <div class="project-item">
    <div class="project-img">
      <img :src="projectOption.url" alt="" />
    </div>
    <p class="project-intro">
      <strong>项目简介：</strong>
      <span v-html="projectOption.intro"></span>
    </p>
    <p class="technology-stack" v-if="projectOption.stack">
      <strong>{{ projectOption.stack }}</strong>
    </p>
    <div class="project-code">
      <a class="sound-code" :href="`https://${projectOption.code}`">
        <strong>项目源码：</strong>{{ projectOption.code }}</a
      >
      <a class="preview" :href="`https://${projectOption.preview}`"
        ><strong>项目预览：</strong>{{ projectOption.preview }}</a
      >
    </div>
    <div class="title">{{projectOption.title}}</div>
  </div>
</template>

<script>
let projectOption = {
  url: "../assets/eazy-ui.png",
  intro:
    "参照 Ant Design、Element UI 等 UI库思路，制作的一个基于 Vue 的简易 UI 组件库。目前已支持Button、Input、Container、Layout、Toast、Tabs、Popover、Collapse等组件。每个组件均经历从需求分析到 Mocha 单元测试，并用TravisCI实现持续集成，最终以 VuePress为基础制作官方文档，发布于 npmjs.org。完成该项目使我循序渐进学会Vue特性，掌握部分设计模式及造轮子技巧。",
  stack: "Vue.js + VuePress + ES6 + Vue CLI + Npm Scripts + Mocha + TravisCI",
  code: "github.com/luckzhu/eazy-ui",
  preview: "luckzhu.github.io/eazy-ui"
};

export default {
  props: {
    projectOption: {
      type: Object,
      default() {
        return projectOption;
      },
      required: true
    }
  }
};
</script>

<style lang="scss">
.project-item {
  width: 100%;
  font-size: 1vw;
  display: flex;
  flex-direction: column;
  position: relative;
  img {
    width: 100%;
    height: auto;
  }
  > * {
    margin-top: 0.2vw;
  }
  .project-intro {
    text-align: justify;
    em {
      color: #009bdf;
      font-weight: bold;
    }
  }
  .technology-stack {
    align-self: center;
    margin: 0.3vw 0;
  }
  .project-code {
    display: flex;
    justify-content: space-between;
  }

  .title {
    width: 10vw;
    height: 3vw;
    background-color: #009bdf;
    border-radius: .2vw;
    color: #fff;
    font-size: 1.2vw;
    position: absolute;
    left: 0;
    top: 0;
   display: flex;
   justify-content: center;
   align-items: center;
  }
}
</style>