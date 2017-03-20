<template>
<el-menu theme="dark" :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
  <el-menu-item index="1">嘿嘿嘿小剧场</el-menu-item>
  <el-submenu index="2">
    <template slot="title">频道</template>
    <el-menu-item index="2-1">大片</el-menu-item>
    <el-menu-item index="2-2">全景</el-menu-item>
    <el-menu-item index="2-3">电视剧</el-menu-item>
    <el-menu-item index="2-1">福利</el-menu-item>
    <el-menu-item index="2-2">美女</el-menu-item>
    <el-menu-item index="2-3">动画</el-menu-item>
  </el-submenu>
  <el-menu-item index="3"><a href="https://www.ele.me" target="_blank">关于我们</a></el-menu-item>
</el-menu>
</template>

<script>
  export default {
    data () {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      }
    },
    methods: {
      handleSelect (key, keyPath) {
        console.log(key, keyPath)
      }
    }
  }
</script>
