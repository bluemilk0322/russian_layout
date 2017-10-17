<template>
<div class="carousel">
  <el-carousel :interval="10000" arrow="always" height="30vh">
    <el-carousel-item v-for="item in 4" :key="item">
      <h3>{{ item }}</h3>
    </el-carousel-item>
  </el-carousel>
</div>
</template>

<style>
    .el-carousel{
        top:10vh;
        left:15vh;
        width: 1200px;
        z-index:-1;
    }
  .el-carousel__item h3 {
    color: #ffffff;
    font-size: 25px;
    opacity: 0.75;
    line-height: 250px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #22313F;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #22313F;
  }
</style>