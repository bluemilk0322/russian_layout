<template>
    <div class = "nav">
        <el-menu theme="dark" :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
            <el-menu-item index="1">最新消息</el-menu-item>
            <el-submenu index="2">
            <template slot="title">系介紹</template>
            <el-menu-item index="2-1">系歷史</el-menu-item>
            <el-menu-item index="2-2">宗旨與目標</el-menu-item>
            <el-menu-item index="2-3">招生資訊</el-menu-item>
            <el-menu-item index="2-4">未來發展</el-menu-item>
            <el-menu-item index="2-5">獎助學金</el-menu-item>
            <el-menu-item index="2-6">交換學生計畫</el-menu-item>
            <el-menu-item index="2-7">辦法及相關表格</el-menu-item>
            </el-submenu>
            <el-submenu index="3">
            <template slot="title">師資陣容</template>
            <el-menu-item index="3-1">師資介紹</el-menu-item>
            <el-menu-item index="3-2">行政人員</el-menu-item>
            </el-submenu>
            <el-submenu index="4">
            <template slot="title">課程資訊</template>
            <el-menu-item index="4-1">課程時間表</el-menu-item>
            <el-menu-item index="4-2">課程規劃</el-menu-item>
            <el-menu-item index="4-3">課程資訊網</el-menu-item>
            <el-menu-item index="4-4">課程大綱查詢系統</el-menu-item>
            </el-submenu>
        </el-menu>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1',
        activeIndex3: '1',
        activeIndex4: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style>
    .nav{
        position:fixed;
        top:13vh;
        left: 30vh;
        width:1000px;
        font-family:"Microsoft YaHei";
        
    }

    .el-menu-item, .el-submenu__title{
      height: 56px;
  line-height: 56px;
  font-size: 18px;
  color: rgb(72, 87, 106);
  padding: 0 20px;
  cursor: pointer;
  position: relative;
  transition: border-color .3s, background-color .3s, color .3s;
  box-sizing: border-box;
  white-space: nowrap;
}

    .el-menu--dark .el-menu-item, .el-menu--dark .el-submenu__title{
      color: #FFFFFF;
    }

    .el-menu--dark{
      background-color: #8DC6FF;
    }

    .el-menu-item.is-active{
      color: #000000;
    }

</style>
