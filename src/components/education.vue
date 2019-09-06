<template>
  <div>
    <div class="column-bar">
      教育经历
    </div>
    <div class="shool-wrapper">
      <div class="school">
        <h4>天津工业大学 纺织学院</h4>
        <p>09/2014~03/2017</p>
      </div>
      <div class="major">
        <h4>非织造材料与工程专业 硕士</h4>
        <p>
          2014--2015 连续两年获得硕士学业奖学金；SCI二区论文一篇（四作），EI
          收录1篇（二作），知网收录2篇。
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
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
  margin-top:1vw;
  h4{
    font-size: 1.1vw;
    font-weight: 500;
    margin-bottom: .3vw;
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