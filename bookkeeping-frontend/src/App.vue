<template>
  <div id="app">
    <div class="page_header">
      <h2>
        <img src="../src/assets/logo.png" alt="bookkeeping">
      </h2>
    </div>
    <div class="page_main">
      <Home></Home>
    </div>
    <div class="page_footer">
      <div class="logo_and_name">
        <img src="../src/assets/logo.png">
        <span>YX Bookkeeping</span>
      </div>
      <div class="website_comment">
        <p>Powered by 远欣记账</p>
        <p>本网站内容版权均归&nbsp;开发者个人&nbsp;所有</p>
        <p>联系电话：13229465045</p>
        <p>更新日期：2022.06.12</p>
      </div>
    </div>
  </div>
</template>

<script>
import Home from '@/components/Home.vue';

export default {
  components: {
    Home,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}
::-webkit-scrollbar {
  /*滚动条整体样式*/
  width: 4px;
  /*高宽分别对应横竖滚动条的尺寸*/
  height: 160px;
}

::-webkit-scrollbar-thumb {
  /*滚动条里面小方块*/
  border-radius: 6px;
  box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2);
  -webkit-box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2);
  background: rgba(144,147,153,.3);
}
.page_header {
  width: 100%;
  height: 60px;
  padding: 0 30px;
  box-sizing: border-box;
  box-shadow: 15px 0px 15px rgba(134, 151, 168, 0.16);
  h2 {
    img {
      width: 130px;
      height: auto;
    }
  }
}
.page_main {
  width: 100%;
  height: calc(100vh - 196px);
}
.page_footer {
  width: 100%;
  height: 136px;
  background: #f0f0f0;
  padding: 0 30px;
  box-sizing: border-box;
  box-shadow: 0px -4px 8px rgba(134, 151, 168, 0.16);
  position: relative;
  .logo_and_name {
    width: 200px;
    img {
      width: 100%;
    }
    span {
      font-size: 20px;
      font-weight: bold;
      line-height: 24px;
      color: #4D4D4D;
      padding-left: 20px;
      box-sizing: border-box;
    }
  }
  .website_comment {
    height: 95px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    p {
      font-size: 16px;
      color: #616161;
      font-weight: bold;
      line-height: 30px;
    }
  }
}
</style>
