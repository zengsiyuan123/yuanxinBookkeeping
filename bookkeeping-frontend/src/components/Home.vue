<template>
  <div class="container">
    <div class="container_left">
      <el-menu
        default-active="2"
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose"
        background-color="#1F2D3D"
        text-color="#BFCBD9"
        active-text-color="#409EFF">
        <el-submenu index="1">
          <template slot="title">
            <i class="el-icon-s-claim"></i>
            <span>明细</span>
          </template>
          <el-menu-item index="1-1">账单</el-menu-item>
          <el-menu-item index="1-2">预算</el-menu-item>
          <el-menu-item index="1-3">资产管家</el-menu-item>
          <el-menu-item index="1-4">理财知识</el-menu-item>
        </el-submenu>
        <el-submenu index="2">
          <template slot="title">
            <i class="el-icon-upload"></i>
            <span>记账</span>
          </template>
          <el-menu-item index="2-1">新增记账</el-menu-item>
          <el-menu-item index="2-2">账单列表</el-menu-item>
        </el-submenu>
        <el-submenu index="3">
          <template slot="title">
            <i class="el-icon-s-data"></i>
            <span>图表</span>
          </template>
          <el-menu-item index="3-1">周</el-menu-item>
          <el-menu-item index="3-2">月</el-menu-item>
          <el-menu-item index="3-3">年</el-menu-item>
        </el-submenu>
        <el-submenu index="4">
          <template slot="title">
            <i class="el-icon-star-on"></i>
            <span>日记</span>
          </template>
          <el-menu-item index="4-1">欣欣日记</el-menu-item>
          <el-menu-item index="4-2">远远日记</el-menu-item>
        </el-submenu>
      </el-menu>
    </div>

    <div class="container_right"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  width: 100%;
  height: 100%;
  overflow-y: auto;
  overflow-x: hidden;
  display: flex;
  justify-content: space-between;
  .container_left {
    width: 160px;
    height: 100%;
    background: #1F2D3D;
    overflow: auto;
    & /deep/ .el-menu {
      height: 100%;
      .el-menu-item {
        min-width: 100%;
      }
    }
  }
}
</style>
