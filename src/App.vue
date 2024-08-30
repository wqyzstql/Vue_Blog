<template>
  <div class="common-layout">
    <el-container>
      <el-header>
        <Headbar/>
      </el-header>
      <el-container class="custom-container">
        <el-aside width='15%' class="border-right">
          <Avator/>
          <Sliderlist/>
        </el-aside>
        <el-container class="main-container">
          <el-main>Main</el-main>
          <el-footer>
            <Footer/>
          </el-footer>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Headbar from './components/headbar.vue'
import Avator from './components/avator.vue';
import Sliderlist from './components/sliderlist.vue'
import Footer from './components/footer.vue';

export default {
  components:{
    Headbar,
    Avator,
    Sliderlist,
    Footer
  }
}
</script>

<style>
.custom-container {
  margin-top: 30px;
  display: flex;
  align-items: stretch;
}
.border-right {
  border-right: 1px solid var(--el-border-color);
}
</style>