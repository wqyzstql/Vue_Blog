<template>
  <div class="common-layout">
    <el-container>
      <el-header>
        <Headbar/>
      </el-header>

      <el-container class="custom-container">
        <el-aside width='15%'>
          <Avator/>
        </el-aside>
        <el-container class="main-container">
          <el-main>Main</el-main>
          <el-footer>Footer</el-footer>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Headbar from './headbar.vue'
import Avator from './avator.vue';

export default {
  components:{
    Headbar,
    Avator
  }
}
</script>

<style>
.custom-container {
  margin-top: 30px;
}
</style>