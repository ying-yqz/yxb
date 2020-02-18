<template>
  <div class="login">
    <div class="login_box">
      <div class="login_text">
        <span>请输入你的生日</span>
      </div>
    </div>

    <div class="password">
      <van-form class="password1">
        <van-field v-model="password" placeholder="YYYY/MM/DD" />
      </van-form>
    </div>

    <div class="big-box" style="position:relative">
      <img class="loginbtn1" src="../../images/btn.png" alt />
      <div class="loginbtn">确认</div>
    </div>
  </div>
</template>

<script>
import {
  //   Tag,
  //   Col,
  //   Icon,
  //   Cell,
  //   CellGroup,
  //   Swipe,
  //   Toast,
  //   SwipeItem,
  //   GoodsAction,
  //   GoodsActionIcon,
  //   GoodsActionButton
  Form,
  Field
} from "vant";

export default {
  components: {
    //   [Tag.name]: Tag,
    //   [Col.name]: Col,
    //   [Icon.name]: Icon,
    //   [Cell.name]: Cell,
    //   [CellGroup.name]: CellGroup,
    //   [Swipe.name]: Swipe,
    //   [SwipeItem.name]: SwipeItem,
    //   [GoodsAction.name]: GoodsAction,
    //   [GoodsActionIcon.name]: GoodsActionIcon,
    //   [GoodsActionButton.name]: GoodsActionButton
    [Form.name]: Form,
    [Field.name]: Field
  },

  data() {
    return {
      password: ""
    };
  },

  methods: {}
};
</script>

<style lang="less">
.login {
  width: 100%;
  height: 80vh;
  // background-color: #f00;
  background-image: url("../../images/科技.jpg");
  padding-top: 20vh;
}
.login_box {
  width: 100%;
  height: 40vh;
  background-image: url("../../images/timg1.png");
  background-repeat: no-repeat;
  background-size: contain;
}
.login_text {
  display: flex;
  height: 28vh;
  justify-content: center;
  align-items: center;
  color: #f00;
  letter-spacing: 2px;
  font-size: 25px;
  // font-family: STKaiti;
  font-family: STFangsong;
  font-weight: 600;
  opacity: 0.8;
  flex-wrap: wrap;
}
.password {
  width: 50%;
  margin: 0 auto;
}
.password1 .van-cell {
  border-radius: 24px;
}
.loginbtn {
  position: absolute;
  top: 20px;
  left: 20px;
  width: 80px;
  height: 80px;
  line-height: 120px;
  border-radius: 40px;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
}
.loginbtn1 {
  // transform: rotate(70deg);
  animation: myfirst 6s infinite linear;
}
@keyframes myfirst {
  0% {
    transform: rotate(360deg);
  }
  25% {
    transform: rotate(720deg);
  }
  50% {
    transform: rotate(1080deg);
  }
  100% {
    transform: rotate(1440deg);
  }
}
.big-box {
  position: relative;
  width: 120px;
  height: 120px;
  margin: 0 auto;
  margin-top: 15px;
  line-height: 120px;
}
</style>
