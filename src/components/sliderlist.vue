<template>
<el-row class="container">
    <el-col>
        <el-link @click="GoGithub">Github</el-link><p></p>
        <el-link>Twitter</el-link>
        <p></p>
        <el-link>osu</el-link>
    </el-col>
</el-row>

</template>

<script setup>
function GoGithub(){
    window.open('https://github.com/wqyzstql', '_blank');
}
</script>

<style>
.container{
    font-size: medium;
    margin-top: 10%;
    text-align: center;
    margin-bottom: 130%;
}
</style>