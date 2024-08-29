<template>
    <el-row class="demo-basic">
      <el-col>
          <div class="block">
            <el-avatar :size="100" :src="circleUrl" />
          </div>
          <div class="sub-title">MyAngelMizuki_</div>
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
    text-align: center;
  }
  .demo-basic .sub-title { 
    margin-bottom: 10px;
    font-size: 14px;
    color: var(--el-text-color-secondary);
  }
  .demo-basic .demo-basic--circle {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .demo-basic .block:not(:last-child) {
    border-right: 1px solid var(--el-border-color);
  }
  .demo-basic .el-col:not(:last-child) {
    border-right: 1px solid var(--el-border-color);
  }
  </style>
  