<template>
<el-footer class="app-footer">
    <div class="footer-content">
        <p>&copy; 2023 Your Company. All rights reserved.</p>
    </div>
</el-footer>
</template>

<script>
export default {
    name: 'Footer',
};
</script>

<style scoped>
.app-footer {
    border-top: 2px solid var(--el-border-color);;
    color: black;
    text-align: center;
    position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
}

.footer-content {
    display: flex;
    flex-direction: column;
    align-items: center;
}
</style>