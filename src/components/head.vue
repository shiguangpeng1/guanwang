<template>
    <div class="head">
        <div class="nav">
            <img class="logo" src="../assets/img/logo.jpg" alt="">
            <el-menu :router="true" :default-active="activeIndex" active-text-color="#417ee4" class="el-menu-demo"
                     mode="horizontal" @select="handleSelect">
                <el-menu-item index="/">首页</el-menu-item>
                <el-menu-item index="/server">产品服务</el-menu-item>
                <el-menu-item index="/case">产品案例</el-menu-item>
                <el-menu-item index="/news">新闻动态</el-menu-item>
                <el-menu-item index="/connect">联系我们</el-menu-item>
                <el-menu-item index="6"><i class="el-icon-phone"></i>176 3003 22755</el-menu-item>
            </el-menu>
        </div>
        <el-carousel :interval="5000" arrow="always">
            <el-carousel-item v-for="item in 4" :key="item">
                <img class="banners" src="../assets/img/banner.jpg" alt="">
            </el-carousel-item>
        </el-carousel>
    </div>

</template>

<script>
    export default {
        data() {
            return {
                activeIndex: '/',
            };
        },
        methods: {
            handleSelect(key, keyPath) {
                console.log(key, keyPath);
            }
        }
    }
</script>

<style lang="scss" scoped>
    .head {
        background-color: #fff;
        .nav {
            height: 100px;
            max-width: 1200px;
            margin: auto;

            .logo {
                float: left
            }

            .el-menu.el-menu--horizontal {
                float: right;
                border-bottom: none;
                padding-top: 39px;

                .el-menu-item {
                    font-size: 16px;
                }
            }
        }
        .banners{
            width: 100%;
        }
    }
</style>