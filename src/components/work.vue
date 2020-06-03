<template>
  <div class="work">
    <div class="column-bar">工作经历</div>
    <div class="shool-wrapper">
      <div class="school">
        <h4>广东省南方名牌产品推进中心</h4>
        <p>09/2019~至今</p>
      </div>
      <div class="major">
        <h4>前端开发工程师</h4>
        <p>前端新项目框架搭建，规范制定，基础组件的编写，二次封装 element-ui 组件。jq 项目的 bug 修复及优化。</p>
      </div>
    </div>
    <div class="shool-wrapper">
      <div class="school">
        <h4>北京知产树教育科技有限公司</h4>
        <p>07/2018~07/2019</p>
      </div>
      <div class="major">
        <h4>运营、设计</h4>
        <p>知识付费、在线教育方向整体的编辑、设计和运营工作。</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.work{
  margin-bottom: 40px;
}
.column-bar {
  background: #e6e7e8;
  font-size: 1.5vw;
  font-weight: 500;
  color: #0f1515;
  padding: 1vw 2.5vw;
}
.shool-wrapper {
  display: flex;
  padding: 0 1.5vw 0 2.5vw;
  font-size: 1.1vw;
  margin-top: 1vw;
  h4 {
    font-size: 1.1vw;
    font-weight: 500;
    margin-bottom: 0.3vw;
  }
  .school {
    white-space: nowrap;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .major {
    margin-left: 3vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
  }
}
</style>