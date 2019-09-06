<template>
  <div id="side-bar">
    <div class="avatar">
      <img src="../assets/My-Picture.png" alt="" />
    </div>
    <div class="primary-information">
      <div class="primary-item">
        <icon name="phone"></icon>
        <span>181 1029 4220</span>
      </div>
      <div class="primary-item">
        <icon name="internet"></icon>
        <span>github.com/luckzhu</span>
      </div>
      <div class="primary-item">
        <icon name="email"></icon>
        <span>luckzhu1992@gmail.com</span>
      </div>
    </div>
    <div class="essential-information">
      <h3 class="information-title">基本信息</h3>
      <p>最高学历<span>:</span>硕士研究生</p>
      <p>毕业时间<span>:</span>2017.03</p>
      <p>出生年月<span>:</span>1992.08</p>
      <p>英语水平<span>:</span>CET-4</p>
    </div>
    <div class="related-skills">
      <h3 class="information-title">相关技能</h3>
      <div class="skills-item">
        <div class="skills-title">JavaScript / HTML 5 / CSS 3</div>
        <div class="skills-bar"></div>
      </div>
      <div class="skills-item">
        <div class="skills-title">Vue.js / Vuex / Vue Router / Axios</div>
        <div class="skills-bar"></div>
      </div>
      <div class="skills-item">
        <div class="skills-title">Node.js</div>
        <div class="skills-bar"></div>
      </div>
      <div class="skills-item">
        <div class="skills-title">Webpack / Parcel / Npm Script</div>
        <div class="skills-bar"></div>
      </div>
      <div class="skills-item">
        <div class="skills-title">ES6 / Scss , Less / Babel</div>
        <div class="skills-bar"></div>
      </div>
      <div class="skills-item">
        <div class="skills-title">Photoshop / Illustrator / Premiere</div>
        <div class="skills-bar"></div>
      </div>
    </div>
    <div class="contact-information">
      <h3 class="information-title">联系方式</h3>
      <div class="contact-item">
        <icon name="shouji"></icon>
        <span>18110294220</span>
      </div>
      <div class="contact-item">
        <icon name="wechat"></icon>
        <span>z6196422</span>
      </div>
      <div class="contact-item">
        <icon name="youxiang"></icon>
        <span>luckzhu1992@gmail.com</span>
      </div>
      <div class="contact-item">
        <icon name="shouye"></icon>
        <span>广州 · 天河区</span>
      </div>
      <div class="contact-item">
        <icon name="github"></icon>
        <span>访问GitHub</span>
      </div>
    </div>
  </div>
</template>

<script>
import Icon from "./icon";
export default {
  data() {
    return {};
  },
  components: {
    Icon
  }
};
</script>

<style lang="scss">
@import "../assets/css/init.scss";
$deepbar: #b7b8b9;
#side-bar {
  display: flex;
  flex-direction: column;
  width: 31vw;
}

.information-title {
  font-size: 1.5vw;
  font-weight: 500;
  color: #0f1515;
  margin-bottom: 1vw;
}

.avatar {
 margin-bottom: -4px;
  img {
    width: 100%;
    height: auto;
  }
}
.primary-information {
  .primary-item {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    color: #fff;
    padding: 1.5vw 2vw;
    &:nth-child(1) {
      background: #00639e;
    }
    &:nth-child(2) {
      background: #007dc5;
    }
    &:nth-child(3) {
      background: #009bdf;
    }

    > span {
      font-size: 1.2vw;
      margin-left: 1.5vw;
    }
    > .icon {
      width: 2vw;
      height: 2vw;
    }
  }
}

.essential-information {
  margin-top: 3vw;
  padding: 0 2vw;
  > p {
    font-size: 1vw;
    margin: 0.5vw 0 0 1vw;
    font-size: 1.2vw;
    > span {
      margin: 0 1.2vw;
    }
  }
}
.related-skills {
  margin-top: 3vw;
  padding: 0 2vw;
  .skills-item {
    margin-top: 0.8vw;
    .skills-title {
      font-family: MyriadPro-It;
      font-size: 1vw;
    }

    .skills-bar {
      height: 1vw;
      background: #b7b8b9;
      position: relative;
      border-radius: 2px;
      &::after {
        content: "";
        height: 1vw;
        background: #009bdf;
        border-radius: 2px;

        position: absolute;
        left: 0;
        top: 0;
      }
    }
    &:nth-child(2) {
      .skills-bar {
        &::after {
          width: 85%;
        }
      }
    }
    &:nth-child(3) {
      .skills-bar {
        &::after {
          width: 65%;
        }
      }
    }
    &:nth-child(4) {
      .skills-bar {
        &::after {
          width: 20%;
        }
      }
    }
    &:nth-child(5) {
      .skills-bar {
        &::after {
          width: 60%;
        }
      }
    }
    &:nth-child(6) {
      .skills-bar {
        &::after {
          width: 50%;
        }
      }
    }
    &:nth-child(7) {
      .skills-bar {
        &::after {
          width: 80%;
        }
      }
    }
  }
}

.contact-information {
  margin-top: 3vw;
  padding: 0 2vw;
  .contact-item {
    margin: 1vw 0 0 1vw;
    display: flex;
    align-items: center;
    > .icon {
      width: 2vw;
      height: 2vw;
    }
    > span {
      font-size: 1.2vw;
      margin: 0 1.2vw;
    }
  }
}
</style>