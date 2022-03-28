<template>
        <!-- 新闻广告 -->
        <div class="m-news">
            <!-- 导航部分 -->
            <div class="part-top-tab">
                <ul class="part-tab-title">
                    <li @mouseover="toggleUl(1)" :class="NavigatioStyle[0]"><i>综合</i><span :style="{display: disp[0].disp}">&#8211;&#9830;&#8211;</span></li>
                    <li @mouseover="toggleUl(2)" :class="NavigatioStyle[1]"><i>公告</i><span :style="{display: disp[1].disp}">&#8211;&#9830;&#8211;</span></li>
                    <li @mouseover="toggleUl(3)" :class="NavigatioStyle[2]"><i>赛事</i><span :style="{display: disp[2].disp}"> &#8211;&#9830;&#8211;</span></li>
                    <li @mouseover="toggleUl(4)" :class="NavigatioStyle[3]"><i>攻略</i><span :style="{display: disp[3].disp}">&#8211;&#9830;&#8211;</span></li>
                    <li @mouseover="toggleUl(5)" :class="NavigatioStyle[4]"><i>社区</i><span :style="{display: disp[4].disp}">&#8211;&#9830;&#8211;</span></li>
                </ul>
            </div>
            <!-- 内容部分 -->
            <div class="new-tab-content">
                <ul class="new-tab-content-ul"  :style="{display: disp[0].disp}">
                    <li class="first"><a href="" class="item-href">福星计划权益皮肤更新公告</a></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线1</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                </ul>
                <ul class="new-tab-content-ul" :style="{display: disp[1].disp}">
                    <li class="first"><a href="" class="item-href">福星计划权益皮肤更新公告</a></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线2</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                </ul>
                <ul class="new-tab-content-ul" :style="{display: disp[2].disp}">
                    <li class="first"><a href="" class="item-href">英雄麦克疯：命悬一线OMG，再冲剁手高天亮</a></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线3</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                </ul>
                <ul class="new-tab-content-ul" :style="{display: disp[3].disp}">
                    <li class="first"><a href="" class="item-href">
              版本答案：刮痧女王阿狸重做后竟变成版本T0中单
            </a></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线4</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                </ul>
                <ul class="new-tab-content-ul" :style="{display: disp[4].disp}">
                    <li class="first"><a href="" class="item-href">联盟趣谈（1）：战斗学院系列皮肤背景故事</a></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣小欣</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线5</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线</a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                    <li class="newsitem inform"><span class="item-type">公告</span><a href="" class="item-href">全新小蜜蜂系列皮肤上线 </a><span class="item-item">03-02</span></li>
                </ul>
                <a target="_blank" class="btn-morenews" href="/news/index.shtml" onclick="PTTSendClick('Notice','Notice-more','阅读更多最新资讯')">
                    <span class="c1">阅读更多</span>
                    <span class="c2">最新资讯</span>
                    <i class="more-arrow"></i>
                 </a>
            </div>
        </div>
</template>

<script>
    export default {
        data(){
           return{
               disp:[
                    {dispId:1,disp:"block"},
                    {dispId:2,disp:"none"},
                    {dispId:3,disp:"none"},
                    {dispId:4,disp:"none"},
                    {dispId:5,disp:"none"}
                ],
                NavigatioStyle:[
                    {nsId:1,liys:true},
                    {nsId:2,liys:false},
                    {nsId:3,liys:false},
                    {nsId:4,liys:false},
                    {nsId:5,liys:false}
                ]
           }
        },
        methods:{
            toggleUl(toggleid){
                this.disp.forEach((dsp,index) => {
                    if (toggleid===dsp.dispId) {
                        this.disp[index].disp = "block";
                    }else{
                        this.disp[index].disp = "none"
                    }
                });
                this.NavigatioStyle.forEach((ns,index) => {
                    if (toggleid===ns.nsId) {
                        this.NavigatioStyle[index].liys = true
                    }else{
                        this.NavigatioStyle[index].liys = false
                    }
                });
            }
        }
    }
</script>

<style scoped>
/* 新闻公告导航部分 */
.m-news {
    width: 496px;
    height: 380px;
    overflow: hidden;
    float: right;
}
.m-news .part-top-tab {
    width: 496px;
    height: 35px;
    overflow: visible;
    box-sizing: border-box;
    border-bottom: 1px #e0e2e2 solid;
}
.m-news .part-tab-title {
    width: 596px;
    height: 35px;
    left: 0;
}
.part-tab-title {
    height: 35px;
    left: 128px;
    box-sizing: border-box;
    border-bottom: 1px #e0e2e2 solid;
}
.m-news .part-tab-title>li {
    font-size: 18px;
    line-height: 24px;
    margin-right: 74px;
}
.liys>i{
    font-weight: 700;
    color: #1da6ba;
}
.part-tab-title>li {
    list-style: none;
    position: relative;
    cursor: pointer;
    float: left;
    width: auto;
    min-width: 40px;
    height: 37px;
    overflow: visible;
    color: #676767;
    font-size: 16px;
    letter-spacing: 1px;
    line-height: 35px;
    text-align: center;
}
.part-tab-title>li>span{
    display: block;
    margin-top: -3px;
    color: #1da6ba;
    display: none;
}
.part-tab-title>li:hover span{
    
    display: block;
}
.part-tab-title>li.selected, .part-tab-title>li:hover {
    font-weight: 700;
    color: #1da6ba;
}
/* 新闻公告内容部分 */
.new-tab-content-ul {
    width: 496px;
    height: 305px;
    position: relative;
}
.new-tab-content-ul>.first {
    list-style: none;
    background-position: 0 -458px;
    width: 496px;
    height: 59px;
    overflow: hidden;
    line-height: 59px;
    text-align: center;
    font-size: 22px;
    font-weight: 700;
    box-sizing: border-box;
    padding: 0 12px;
    text-overflow: ellipsis;
    white-space: nowrap;
    color: #0da0b4;
}
.new-tab-content-ul>.first>.item-href {
    color: #0da0b4;
    font-size: 22px;
    font-weight:bold;
}
a {
    text-decoration: none;
}
.newsitem {
    list-style: none;
    width: 496px;
    height: 40px;
    line-height: 39px;
    overflow: hidden;
    box-sizing: border-box;
    border-top: 1px #e0e2e2 solid;
    text-align: left;
}
.newsitem>.item-type {
    display: inline-block;
    vertical-align: middle;
    *zoom: 1;
    *display: inline;
    width: 36px;
    height: 20px;
    box-sizing: border-box;
    font-size: 12px;
    border: 1px #69c5d2 solid;
    color: #1da6ba;
    line-height: 18px;
    text-align: center;
}
.newsitem>.item-href {
    display: inline-block;
    vertical-align: middle;

    width: 370px;
    height: 39px;
    line-height:39px;
    overflow: hidden;
    margin-left: 20px;
    color: #424242;
    font-size: 16px;
    letter-spacing: 1px;
    text-overflow: ellipsis;
    white-space: nowrap;
}
.newsitem>.item-item{
    vertical-align: middle;
    margin-left: 16px;
    text-align: left;
    overflow: hidden;
    color: #9d9d9d;;
    font-size: 16px;
}
.btn-morenews{
    display: block;
    width: 496px;
    height: 40px;
    overflow: hidden;
    background-color: #e3e2e2;
    position: relative;
    line-height: 40px;
    text-align: center;
}
.btn-morenews>.c1 {
    font-size: 14px;
    color: #676767;
}
.btn-morenews>.c2 {
    font-size: 14px;
    color: #7ea1a6;
}

</style>