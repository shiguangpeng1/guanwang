<template>
    <div class="content">
        <div class="top">
            <div>
                <h1 class="title">用心服务 追求客户满意</h1>
                <h3 class="sub_title">技术跨界，创意自由。专业APP研发</h3>
                <div class="serve">
                    <el-row>
                        <el-col :span="6">
                            <i class="iconfont icon-computer_icon"></i>
                            <p>[品牌网站建设]</p>
                            <span class="sub">BRAND WEBSITE CONSTRUCTION</span>
                        </el-col>
                        <el-col :span="6">
                            <i class="iconfont icon-phone_icon"></i>
                            <p>[专业APP定制]</p>
                            <span class="sub">PROFESSIONAL APP CUSTOMIZATION</span>
                        </el-col>
                        <el-col :span="6">
                            <i class="iconfont icon-xiaochengxu"></i>
                            <p>[微信小程序定制开发]</p>
                            <span class="sub">SMALL PROGRAM CUSTOM DEVELOPMENT</span>
                        </el-col>
                        <el-col :span="6">
                            <i class="iconfont icon-xietongyanfa"></i>
                            <p>[软件研发]</p>
                            <span class="sub">SOFTWARE DEVELOPMENT</span>
                        </el-col>
                    </el-row>
                </div>

                <div class="detail clear">
                    <div>
                        <i class="iconfont icon-tuandui"></i>
                        <p></p>
                    </div>
                    <div>
                        <i class="iconfont icon-anli"></i>
                        <p></p>
                    </div>
                    <div>
                        <i class="iconfont icon-sheji"></i>
                        <p></p>
                    </div>
                    <div>
                        <i class="iconfont icon-shouru"></i>
                        <p></p>
                    </div>
                    <div>
                        <i class="iconfont icon-dingshi"></i>
                        <p></p>
                    </div>
                    <div>
                        <i class="iconfont icon-RNicon"></i>
                        <p></p>
                    </div>
                    <div>
                        <i class="iconfont icon-huzhu"></i>
                        <p></p>
                    </div>
                </div>
            </div>
        </div>
        <div class="sort">
            <h1 class="title">为您量身打造原生APP</h1>
            <h3 class="sub_title">我们认真服务好每一位客户，让客户满意是我们的宗旨</h3>
            <div class="clear">
                <div class="item" v-for="i in 6" :key="i">
                    <div>
                        <i class="iconfont icon-canyin"></i>
                        <p>餐饮外卖</p>
                        <p class="sub">餐饮展示、美食展示、定位就餐、用餐评价、</p>
                    </div>

                </div>
            </div>
        </div>
        <div class="about">
            <div>
                <h2>我们是设计师、工程师、梦想者<br>也是您的用户体验专家</h2>
                <p>透视互联专注于APP定制研发及高校就业管理系统为业务核心。致力于为企事业单位、学校、政府机构提供信息化服务。服务范围包括：高校就业管理系统、移动APP、微信定制开发、网站建设、SME托管运营、超高性能纤维混凝土、医院自助终端机、远程试衣等。目前与多家企事业单位保持良好的合作关系。我们的价值与宗旨是为用户和客户...</p>
                <router-link class="about_more" to="/">了解更多</router-link>
            </div>

        </div>
        <div class="news">
            <h1 class="title">新闻动态</h1>
            <h3 class="sub_title">团队活动&nbsp;/&nbsp;更新案例&nbsp;/&nbsp;项目动态</h3>
            <div>
                <div>
                    <img src="@/assets/demo/new.jpg" alt="">
                </div>
                <div class="right">
                    <div class="act">NEWS 新闻咨询</div>
                    <div>NEWS 新闻咨询</div>
                    <div>NEWS 新闻咨询</div>
                    <div>NEWS 新闻咨询</div>
                    <div>NEWS 新闻咨询</div>
                    <div>NEWS 新闻咨询</div>
                </div>
            </div>
        </div>
        <div class="partner">
            <h1 class="title">他们选择了透视互联</h1>
            <h3 class="sub_title">团队活动&nbsp;/&nbsp;更新案例&nbsp;/&nbsp;项目动态</h3>
            <div>

            </div>
        </div>
    </div>
</template>

<script>

    export default {
        data() {
            return {
                sort: [
                    {
                        img: require("../assets/demo/canyin.png"),
                        img_foc: require("../assets/demo/canyin_foc.png"),
                        act: false,
                        bg:'#fff',
                        act_bg: "#f0a228",
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .content {
        text-align: center;

        .top {
            background-color: #fff;
            border: 1px solid #fff;

            > div {
                width: 1200px;
                margin: auto;

                .title {
                    color: #417ee4;
                    border-bottom: 2px solid #f5f5f5;
                }

                .sub_title {
                    color: #999999;
                }

                .serve {
                    .iconfont {
                        display: block;
                        width: 100px;
                        height: 100px;
                        margin: 30px auto 0;
                        border: 2px solid #b6cdf5;
                        -webkit-border-radius: 50%;
                        -moz-border-radius: 50%;
                        border-radius: 50%;
                        line-height: 100px;
                        font-size: 50px;
                        color: #4888f4;
                        transition: all .5s;
                    }

                    .iconfont:hover {
                        border-color: #417ee4;
                        background-color: #417ee4;
                        color: #fff;
                    }

                    .sub {
                        font-size: 14px;
                        color: #c1c1c1;
                        word-break: break-all;
                    }
                }

                .detail {
                    width: 80%;
                    margin: 20px auto;

                    div {
                        float: left;
                        width: 14.28%;

                        .iconfont {
                            display: block;
                            width: 50px;
                            height: 50px;
                            margin: auto;
                            line-height: 50px;
                            font-size: 26px;
                            border: 1px solid #ccc;
                            -webkit-border-radius: 50%;
                            -moz-border-radius: 50%;
                            border-radius: 50%;
                            color: #ccc;
                            transition: all .5s;
                        }

                        .iconfont:hover {
                            color: #fff;
                            background-color: #ccc;
                            border-color: #ccc;
                        }
                    }
                }
            }

        }

        .sort {
            background-color: #f9fafc;

            .title {
                color: #417ee4;
            }

            .sub_title {
                color: #999999;
            }

            > div {
                width: 1200px;
                margin: auto;

                .item {
                    float: left;
                    width: 33.33%;
                    margin-bottom: 20px;

                    div {
                        width: 90%;
                        margin: auto;
                        background-color: #fff;
                        padding: 30px 0;
                        transition: all .5s;
                        .iconfont{
                            font-size: 50px;
                            color:#F0A228;
                        }

                        .sub {
                            color: #b4b4b4;
                            font-size: 14px;
                        }
                    }
                    div:hover{
                        background-color: #f0a228;
                        .iconfont{
                            color:#fff;
                        }
                        p{
                            color:#fff;
                        }
                    }
                }
            }
        }
        .about{
            background-color: rgba(0,0,0,.5);
            padding: 40px 0;
            >div{
                width: 1200px;
                margin: auto;
                h2{color:#fff}
                >p{
                    width: 960px;
                    margin: auto;
                    text-align: left;
                    text-indent: 2em;
                    color:#fff;
                }
                .about_more{
                    display: block;
                    margin: 40px auto 0;
                    width: 100px;
                    height: 30px;
                    -webkit-border-radius: 60px;
                    -moz-border-radius: 60px;
                    border-radius: 60px;
                    border:2px solid #fff;
                    color: #fff;
                    font-size: 16px;
                    line-height: 32px;
                    text-decoration: none;
                }
            }
        }
        .news{
            .title {
                color: #417ee4;
            }

            .sub_title {
                color: #999999;
            }
            >div{
                margin: 0 auto 60px;
                width: 1200px;
                height: 300px;
                >div{
                    float: left;
                    width: 590px;
                }
                .right{

                    float: right;
                    div{
                        height: 50px;
                        line-height: 50px;
                        text-align: left;
                        padding: 0 20px;
                        box-sizing: border-box;
                        border: 1px solid #ccc;
                        border-bottom: none;
                        transition: all .3s;
                    }
                    div:last-child{
                        border-bottom: 1px solid #ccc;
                    }
                    div.act{
                        background-color: #417ee4;
                        color:#fff;
                    }
                    div:hover{
                        background-color: #417ee4;
                        color:#fff;
                    }
                }
            }
        }
    }

</style>