<template>
  <div>
    <div class="header-wrapper">
      <h1>朱承章</h1>
      <h2>应聘WEB前端开发</h2>
      <div class="personal-advantage">
        <p>
         <i> 1.</i> 熟练 HTML
          5和常用CSS3，有较好的设计能力，能根据设计图像素级完成页面制作;
        <p>
          <i> 2.</i> 熟悉原生 JavaScript，会使用 ES6+ 常用规范，了解原型， 闭包，
          作用域链等概念;
        </p>
        <p>
         <i> 3.</i> 熟悉
          Vue 框架及常用库的使用，理解如生命周期、组件、虚拟
          DOM、数据响应式等概念， 能够使用 Vue 全家桶（Vue-Cli、Vuex、Vue
          Router）开发项目;
        </p>
        <p>
          <i> 4.</i> 有移动端开发经验，会使用REM、vw/ vh、响应式
          等技术制作适配手机设备的页面;
        </p>
        <p>
          <i> 5.</i> 了解 HTTP 相关知识，了解常见的 Web
          性能优化方案;
        </p>
         <p>
         <i> 6.</i> 熟练使用 VsCode、WebStorm、Scss、Git 等开发工具。
        </p>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.header-wrapper {
  padding: 2vw 2.5vw;
  > h1 {
    font-size: 3vw;
    color: #007dc5;
  }
  > h2 {
    font-size: 1.5vw;
    color: #009bdf;
    margin-bottom: 0.8vw;
  }
  .personal-advantage {
    > p {
      font-size: 1vw;
      margin-top: 0.3vw;
      > i {
        font-size: 1.4vw;
        font-weight: 500;
        color: #009bdf;
      }
    }
  }
}
</style>