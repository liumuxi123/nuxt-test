<template>
  <div>
    <el-menu
      default-active="1"
      class="el-menu-demo"
      mode="horizontal"
    >
      <el-menu-item index="1">
        <nuxt-link to="/">首页</nuxt-link>
      </el-menu-item>
      <el-menu-item index="2">
        <nuxt-link to="/user">用户中心</nuxt-link>
      </el-menu-item>
      <el-submenu index="3">
        <template slot="title">商品管理</template>
        <el-menu-item index="3-1">
          <nuxt-link to="/good">商品列表</nuxt-link>
        </el-menu-item>
        <el-menu-item index="3-2">
          <nuxt-link to="/good/:id">商品详情</nuxt-link>
        </el-menu-item>
      </el-submenu>
    </el-menu>
    <Nuxt />
  </div>
</template>

<script>
export default {
  // middleware:'auth',
}
</script>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
