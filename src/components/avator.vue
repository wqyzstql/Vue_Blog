<template>
    <el-row class="demo-basic">
      <el-col>
          <div class="block">
            <el-avatar :size="100" :src="circleUrl" />
          </div>
          <div class="sub-title">MyAngelMizuki_</div>
          <div class="sign">个性签名区</div>
      </el-col>
    </el-row>
  </template>
  <script lang="ts" setup>
  import { reactive, toRefs } from 'vue'
  
  const state = reactive({
    circleUrl:
      'https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png',
  })
  const { circleUrl } = toRefs(state)
  </script>
  
  <style scoped>
  .demo-basic {
    margin-top: 30%;
    text-align: center;
  }
  .demo-basic .sign{
    font-size: small;
    margin-bottom: 30px;
  }
  .demo-basic .sub-title { 
    margin-top: 30px;
    margin-bottom: 10px;
    font-size: 18px;
    color:black;
    font-weight: bold;
  }
  .demo-basic .demo-basic--circle {
    justify-content: space-between;
    align-items: center;
  }
  </style>
  