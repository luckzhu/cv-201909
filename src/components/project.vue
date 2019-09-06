<template>
  <div>
    <div class="project-wrapper">
      <div class="column-bar">
        项目经历
      </div>
      <div class="items" v-for="item in projectItemOption">
        <projectItem :projectOption="item"></projectItem>
      </div>
    </div>
  </div>
</template>

<script>
let projectItemOption = [
  {
    url: require("../assets/eazy-ui.png"),
    intro:
      "参照 Ant Design、Element UI 等 UI库思路，制作的一个基于 Vue 的简易 UI 组件库。目前已支持Button、Input、Container、Layout、Toast、Tabs、Popover、Collapse等组件。每个组件均经历从需求分析到 Mocha 单元测试，并用TravisCI实现持续集成，最终以 VuePress为基础制作官方文档，发布于 npmjs.org。完成该项目使我循序渐进学会Vue特性，掌握部分设计模式及造轮子技巧。",
    stack: "Vue.js + VuePress + ES6 + Vue CLI + Npm Scripts + Mocha + TravisCI",
    code: "github.com/luckzhu/eazy-ui",
    preview: "luckzhu.github.io/eazy-ui"
  },
  {
    url: require("../assets/cnode.png"),
    intro:
      "该项目使用 Vue 制作 CNode 官方社区全新UI重置版，并做了响应式适配，调用 CNode 官方社区提供的 API，以 Vue CLI 创建项目模版，二次封装 Axios 获取数据，使用 Vue Router 进行前端路由的切换及传参，使用 watch 监听路由的变化，Webpack 打包。",
    stack: "Vue CLI/ Vue2/ Vue Router/ Axios/ ES6/ Npm/ SCSS",
    code: "github.com/luckzhu/cnode",
    preview: "luckzhu.github.io/cnode-preview"
  },

  {
    url: require("../assets/blog-client.png"),
    intro:
      "该项目使用 Vue 实现了一个在线博客分享的平台。包含首页、用户文章列表、个人管理等页面，实现了登录、注册、编辑、发布等功能。项目使用 Grid 作页面布局，以 Vue CLI 为基础创建项目模版，使用 Less 作 CSS 预处理，引用 Element UI 作交互。通过 Vue Router 实现路由的跳转、异步加载、权限验证等，通过 vuex 实现状态管理，用 Axios 获取数据，并对接口进行了封装。",
    stack: "Vue CLI/ Vue2/ Axios/ Vue Router/ Vuex/ ES6/ Npm/ Grid/ Less",
    code: "github.com/luckzhu/blog-client",
    preview: "luckzhu.github.io/blog-client-preview"
  },

  {
    url: require("../assets/canvas.png"),
    intro:
      "是一个使用纯原生 JS 开发的，主要利用 HTML 5 的 Canvas API ，是我在学习原生 JS 及 Canvas 过程中开发的小工具。 其提供在 PC 及手机端在线画画、橡皮擦、画笔调色、画作删除等功能，并支持画作下载。",
    stack: "",
    code: "github.com/luckzhu/canvas",
    preview: "luckzhu.github.io/canvas"
  },
  {
    url: require("../assets/auto-drawing.png"),
    intro:
      "是一个使用纯原生 JS 开发的，动态显示 CSS 画一个小黄人头部过程的小作品。该作品主要思路是通过间隔计时器遍历预先设置在 preview 标签内代码，将其一个个显示在页面上，并在 style 标签上作同样处理，以使代码 CSS 生效。此外，实现了 CSS 高亮效果及调速功能。",
    stack: "",
    code: "github.com/luckzhu/auto-draw",
    preview: "luckzhu.github.io/auto-draw"
  }
];

import projectItem from "./project-item.vue";

export default {
  data() {
    return {
      projectItemOption
    };
  },
  components: {
    projectItem
  }
};
</script>

<style lang="scss">
.project-wrapper {
  display: flex;
  flex-direction: column;
  .column-bar{
    margin-bottom: 2.5vw;
  }
  .items {
    padding: 2.5vw;
    padding-top: 0;

  }
}
</style>