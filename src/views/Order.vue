<template>
  <div>
    <header class="header">
      <span>{{ arrow }}</span>
      <span>确认订单</span>
      <span></span>
    </header>
    <main class="main">
      <div class="address-wrapper">
        <div class="top">
          <span class="top-left">取</span>
          <div class="top-center">
            <div>取车网点</div>
            <div>乐儿会超市停车场</div>
          </div>
          <span class="top-right">{{ arrow1 }}</span>
        </div>
        <div class="mid">
          <div class="mid-left">还</div>
          <div class="mid-center">
            <div class="text-wrapper">
              <span>可还至有剩余车位的任意网点</span>
              <span>(异地还车会收取费用)</span>
            </div>
            <div class="net-wrapper">
              <span>六安市</span>
              <span class="triangle-bottom"></span>
              <span>网点分布</span>
              <span class="triangle-right"></span>
            </div>
          </div>
          <div class="mid-right"></div>
        </div>
        <div class="bottom">
          <div class="bottom-left">T</div>
          <div class="bottom-center">
            <div>租期【共7天】</div>
            <div>06月26日 10:00 - 07月03日 10:00</div>
          </div>
          <div class="bottom-right"></div>
        </div>
      </div>
      <div class="money-wrapper">
        <div class="top">
          <span class="top-left">基本服务</span>
          <span class="top-center">收费项目说明</span>
          <span class="top-right">i</span>
        </div>
        <div class="center">
          <div class="div1">
            <span>车辆租金</span>
            <span>37×7.00=</span>
            <span>257元</span>
          </div>
          <div class="div2">
            <span>手续费</span>
            <span>20×1=</span>
            <span>20元</span>
          </div>
          <div class="div3">
            <span>基本服务费</span>
            <span>40×7=</span>
            <span>280元</span>
          </div>
          <div class="div4">
            <span>推荐服务</span>
            <span></span>
            <span></span>
          </div>
          <div class="div5">
            <span>无忧服务费<span class="question">?</span></span>
            <span>50×7=</span>
            <span>350元<span class="circle"></span></span>
          </div>
        </div>
      </div>
      <div class="active-wrapper">
          <span>参与优惠活动</span>
          <span>日租新用户福利-首日0租金</span>
          <span>{{arrow1}}</span>
      </div>
      <div class="deposit-wrapper">
          <div class="top">
              <span>请选择押金方式</span>
              <span>免押规则</span>
              <span>i</span>
          </div>
          <div class="bottom">
              <span>支付押金</span>
              <span>芝麻免押</span>
          </div>
      </div>
      <div class="count-wrapper">
          <div>订单合计:<span class="count">557</span>元</div>
          <div>套餐说明:提前换车不退款 续租按日租计费 油费自理</div>
      </div>
    </main>
  </div>
</template>

<script lang="js">
export default {
    data(){
        return{
           arrow:'<',
           arrow1:'>' 
        }
    }
}  
</script>
<style scoped lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 16px;
  font-size: 18px;
  font-weight: 600;
}
.address-wrapper {
  background: white;
  border-radius: 20px;
  margin: 10px;
  padding: 16px;
  > .top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    > .top-left {
      background: rgb(0, 0, 68);
      border-radius: 50%;
      padding: 2px 4px;
      color: white;
      font-size: 12px;
    }
    > .top-center {
      margin-right: auto;
      padding-left: 10px;
      text-align: left;
      div:nth-child(1) {
        color: rgb(15, 155, 197);
        font-size: 12px;
      }
      div:nth-child(2) {
        font-size: 14px;
        padding-top: 6px;
      }
    }
    > .top-right {
      font-size: 18px;
      font-weight: 600;
    }
  }
  .mid {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
    > .mid-left {
      background: rgb(0, 0, 68);
      border-radius: 50%;
      padding: 2px 4px;
      color: white;
      font-size: 12px;
    }
    > .mid-center {
      margin-right: auto;
      padding-left: 10px;
      text-align: left;
      > .text-wrapper {
        font-size: 12px;
        span:nth-child(1) {
          color: rgb(15, 155, 197);
        }
        span:nth-child(2) {
          color: red;
        }
      }
      > .net-wrapper {
        font-size: 14px;
        padding-top: 6px;
        display: flex;

        > .triangle-bottom {
          width: 0;
          height: 0;
          border: 6px solid transparent;
          border-top: 6px solid rgb(158, 158, 160);
          align-self: flex-end;
          margin: 0 6px;
        }
        > .triangle-right {
          width: 0;
          height: 0;
          border: 6px solid transparent;
          border-left: 6px solid rgb(158, 158, 160);
          align-self: center;
          margin: 0 6px;
        }
      }
    }
  }
  .bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
    > .bottom-left {
      background: rgb(0, 0, 68);
      border-radius: 50%;
      padding: 2px 6px;
      color: white;
      font-size: 16px;
    }
    > .bottom-center {
      margin-right: auto;
      padding-left: 10px;
      text-align: left;
      div:nth-child(1) {
        color: rgb(15, 155, 197);
        font-size: 12px;
      }
      div:nth-child(2) {
        font-size: 14px;
        padding-top: 6px;
      }
    }
  }
}
.money-wrapper {
  background: white;
  border-radius: 20px;
  margin: 10px;
  padding: 16px;
  > .top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    > .top-left {
      font-size: 16px;
      font-weight: 600;
    }
    > .top-center {
      color: rgb(15, 155, 197);
      margin-left: auto;
      text-align: right;
    }
    > .top-right {
      border: 1px solid rgb(15, 155, 197);
      border-radius: 50%;
      padding: 2px 8px;
      color: rgb(15, 155, 197);
      font-size: 14px;
      margin-left: 10px;
    }
  }
  > .center {
    margin-top: 20px;
    > .div1,
    .div2,
    .div3,
    .div4,
    .div5 {
      display: flex;
      justify-content: space-between;
      padding: 4px 2px;
      span:nth-child(1) {
        font-size: 16px;
        font-weight: 600;
        > .question {
          background: rgb(0, 0, 68);
          border-radius: 50%;
          padding: 0 2px;
          color: white;
          font-size: 12px;
          margin-left: 6px;
        }
      }
      span:nth-child(2) {
        font-size: 18px;
        color: rgb(192, 192, 192);
      }
      span:nth-child(3) {
        font-size: 16px;
        font-weight: 600;
        > .circle {
          border: 1px solid rgb(192, 192, 192);
          border-radius: 50%;
          padding: 4px 12px;
          margin-left: 8px;
        }
      }
    }
  }
}
.active-wrapper{
  background: white;
  border-radius: 20px;
  margin: 10px;
  padding: 16px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  span:nth-child(1){
    font-size: 18px;
    font-weight: 600;
  }
  span:nth-child(2){
    color: rgb(15, 155, 197);
    margin-left: auto;
    text-align: right;
    font-size: 14px;
  }
  span:nth-child(3){
    font-size: 18px;
    font-weight: 600;
    margin-left: 14px;
    padding-top: 2px;
  }
}
.deposit-wrapper{
  background: white;
  border-radius: 20px;
  margin: 10px;
  padding: 16px;
  > .top{
      display: flex;
      justify-content: space-between;
      align-items: center;
      span:nth-child(1){
        font-size: 18px;
        font-weight: 600;
      }
      span:nth-child(2){
        color: rgb(15, 155, 197);
        margin-left: auto;
        text-align: right;
        font-size: 14px;
      }
      span:nth-child(3){
        border: 1px solid rgb(15, 155, 197);
        border-radius: 50%;
        padding: 2px 8px;
        color: rgb(15, 155, 197);
        font-size: 14px;
        margin-left: 8px; 
      }
  }
  > .bottom{
      display: flex;
      justify-content: space-around;
      align-items: center;
      margin-top: 20px;
      span:nth-child(1){
        width: 50%;
        background: rgb(221, 221, 221);
        border-radius: 100px / 85px;
        padding: 10px;
        margin: 0 4px;
      }
      span:nth-child(2){
        width: 50%;
        background: rgb(255, 255, 255);
        border: 1px solid rgb(15, 155, 197);
        border-radius: 100px / 100px;
        padding: 10px;
        margin: 0 4px;
      }
  }
}
.count-wrapper{
  background: white;
  border-radius: 20px;
  margin: 10px;
  padding: 16px;
  display: flex;
  flex-direction: column;
  div:nth-child(1){
      font-size: 16px;
      text-align: left;
      font-weight: 600;
      >.count{
         font-size: 24px; 
         padding-left: 4px;
      }
  }
  div:nth-child(2){
      font-size: 12px;
      text-align: left;
      color: rgb(15, 155, 197);
      margin-top: 10px;
  }
}
</style>

