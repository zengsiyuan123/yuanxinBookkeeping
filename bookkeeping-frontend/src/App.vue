<template>
  <div id="app">
    <div class="page_header">
      <h2>Bookkeeping</h2>
    </div>
    <div class="page_main">
      <Home></Home>
    </div>
    <div class="page_footer">
      <p>底部网站简介</p>
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
// ::-webkit-scrollbar {
//   /*滚动条整体样式*/
//   width: 4px;
//   /*高宽分别对应横竖滚动条的尺寸*/
//   height: 160px;
// }

// ::-webkit-scrollbar-thumb {
//   /*滚动条里面小方块*/
//   border-radius: 6px;
//   box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2);
//   -webkit-box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2);
//   background: #FFF;
// }
.page_header {
  width: 100%;
  height: 60px;
  background: #4090FF;
  padding: 0 30px;
  box-sizing: border-box;
  h2 {
    font-size: 20px;
    color: #000;
    font-weight: bold;
    line-height: 60px;
  }
}
.page_main {
  width: 100%;
  height: calc(100vh - 120px);
}
.page_footer {
  width: 100%;
  height: 60px;
  background: cadetblue;
  padding: 0 30px;
  box-sizing: border-box;
  p {
    font-size: 20px;
    color: #000;
    font-weight: bold;
    line-height: 60px;
  }
}
</style>
