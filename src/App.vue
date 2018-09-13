<template>
  <div id="app">
    <el-container>
      <el-header class="header">
        <vheader></vheader>
      </el-header>
      <el-container>
        <el-aside width="200px">
          <nav_menu></nav_menu>
        </el-aside>
        <el-main>
          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>

  </div>
</template>

<script>
import NavMenu from '@/components/NavMenu'
import Header from '@/components/Header'

export default {
  name: 'App',
  components: {
    'nav_menu': NavMenu,
    'vheader': Header
  }
}
</script>

<style>
  .header {
    background-color: #409EFF;
    color: #fff;
    line-height: 60px;
  }
/*#app {*/
  /*font-family: 'Avenir', Helvetica, Arial, sans-serif;*/
  /*-webkit-font-smoothing: antialiased;*/
  /*-moz-osx-font-smoothing: grayscale;*/
  /*text-align: center;*/
  /*color: #2c3e50;*/
  /*margin-top: 60px;*/
/*}*/
</style>
