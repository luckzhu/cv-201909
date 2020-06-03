<template>
  <div>
    <div class="project-wrapper">
      <div class="column-bar">项目经历</div>
      <div class="items" v-for="item in projectItemOption" :key="item.url">
        <projectItem :projectOption="item"></projectItem>
      </div>
    </div>
  </div>
</template>

<script>
let projectItemOption = [
  {
    url: require("../assets/dashboard.jpg"),
    title: "数据管理后台",
    intro:
      "基于 vue-element-admin 的基础模板设计开发，实现前端<em>权限控制</em>，根据路由自动生成左侧菜单，<em>iconfont</em> 图标管理，axios <em>全局请求响应的封装</em>。对常用的table（表格）、form（表单）、upload（上传）、exportExcel（导出excel）等 element-ui 组件进行<em>二次封装</em>，大大<em>提高开发效率</em>。",
    stack: "Vue.js/ ElementUi/ ES6/ Vue CLI/ Axios/ Iconfont ",
    preview: "hz.gdclz.org"
  },
  {
    url: require("../assets/nj-echarts.jpg"),
    title: "数据可视化",
    intro:
      "使用 <em>echarts</em> 展示各类数据图形，如柱状图、饼图、省市地图、水滴图和雷达图等。数据变化时图形自动<em>响应变化</em>，全屏切换，两种配色<em>风格模式切换</em>。使用 px2rem， 图形跟随屏幕大小进行<em>自动切换</em>。",
    stack: "Vue CLI/ Vue2/ Echarts/ Axios/ Vue Router/ Vuex/ ES6/ px2rem",
    preview: "hz.gdclz.org/nyjyChart/index.html"
  },
  {
    url: require("../assets/eazy-ui.png"),
    title: "简易UI组件库",
    intro:
      "参照 Ant Design、Element UI 等 UI库思路，制作的一个基于 <em>Vue 的简易 UI 组件库</em>。目前已支持Button、Input、Container、Layout、Toast、Tabs、Popover、Collapse等组件。每个组件均经历从需求分析到 <em>Mocha 单元测试</em>，并用 <em>TravisCI 实现持续集成</em>，最终以 <em>VuePress</em>为基础制作官方文档，发布于 <em>npmjs.org</em>。完成该项目使我循序渐进学会Vue特性，掌握部分设计模式及造轮子技巧。",
    stack: "Vue.js/ VuePress/ ES6/ Vue CLI/ Npm Scripts/ Mocha/ TravisCI",
    code: "github.com/luckzhu/eazy-ui",
    preview: "luckzhu.github.io/eazy-ui"
  },
  {
    url: require("../assets/cnode.png"),
    title: "重构 CNode",
    intro:
      "该项目使用 Vue 制作 CNode 官方社区<em>全新UI重置版</em>，并做了<em>响应式适配</em>，调用 CNode 官方社区提供的 API，以 <em>Vue CLI</em> 创建项目模版，<em>二次封装 Axios</em> 获取数据，使用 <em>Vue Router</em> 进行前端路由的切换及传参，使用 watch 监听路由的变化，<em>Webpack 打包</em>。",
    stack: "Vue CLI/ Vue2/ Vue Router/ Axios/ ES6/ Npm/ SCSS",
    code: "github.com/luckzhu/cnode",
    preview: "luckzhu.github.io/cnode-preview"
  },

  {
    url: require("../assets/blog-client.png"),
    title: "博客分享平台",
    intro:
      "该项目使用 Vue 实现了一个<em>在线博客分享</em>的平台。包含首页、用户文章列表、个人管理等页面，实现了登录、注册、编辑、发布等功能。项目使用 <em>Grid 作页面布局</em>，以 Vue CLI 为基础创建项目模版，使用 <em>Scss 作 CSS 预处理</em>，引用 <em>Element UI 作交互</em>。通过 Vue Router 实现路由的跳转、异步加载、权限验证等，通过 <em>vuex 实现状态管理</em>，用 Axios 获取数据，并对接口进行了封装。",
    stack: "Vue CLI/ Vue2/ Axios/ Vue Router/ Vuex/ ES6/ Npm/ Grid/ Less",
    code: "github.com/luckzhu/blog-client",
    preview: "luckzhu.github.io/blog-client-preview"
  },

  {
    url: require("../assets/canvas.png"),
    title: "简易在线画板",
    intro:
      "是一个使用<em>纯原生 JS</em> 开发的，主要利用 HTML 5 的 <em>Canvas API</em> ，是我在学习原生 JS 及 Canvas 过程中开发的小工具。 其提供在 <em>PC 及手机端</em>在线画画、橡皮擦、画笔调色、画作删除等功能，并<em>支持画作下载</em>。",
    stack: "",
    code: "github.com/luckzhu/canvas",
    preview: "luckzhu.github.io/canvas"
  },
  // {
  //   url: require("../assets/auto-drawing.png"),
  //   title: "可爱的小黄人",
  //   intro:
  //     "是一个使用<em>纯原生 JS</em> 开发的，<em>动态显示 CSS </em>画一个小黄人头部过程的小作品。该作品主要思路是通过间隔计时器遍历预先设置在 preview 标签内代码，将其一个个显示在页面上，并在 style 标签上作同样处理，以使代码 CSS 生效。此外，实现了<em> CSS 高亮效果及调速功能</em>。",
  //   stack: "",
  //   code: "github.com/luckzhu/auto-draw",
  //   preview: "luckzhu.github.io/auto-draw"
  // }
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
  .column-bar {
    margin-bottom: 2.5vw;
  }
  .items {
    padding: 2.5vw;
    padding-top: 0;
  }
}
</style>