<template>
  <div class="g-zoombox" style="zoom: 0.879944">
    <div class="g-index-wrap1">
      <!-- 轮播图 -->
      <Carousel />
      <!-- 新闻广告 -->
      <NewsAds />
      <!-- 活动 -->
      <Activity />
      <!-- 游戏功能导航 -->
      <div class="m-gamefunc-nav" exposure-tag="gameNav,游戏功能导航">
        <ul class="slide-nav-ul">
          <li class="herf-download" title="下载游戏">
            <video
              class="side-down-video"
              autoplay=""
              loop=""
              muted=""
              width="366"
              height="168"
            >
              <source
                src="//ossweb-img.qq.com/images/lol/v3/btn-download.mp4"
                type="video/mp4"
              />
            </video>
            <a
              href="download.shtml?ADTAG=lolweb.v3"
              class="herf-mask"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-download','下载游戏')"
              >下载游戏</a
            >
          </li>
          <li class="btn-flashmen p1" title="新手必备">
            新手必备
            <div class="inner-hover">
              <a
                href="/data/newbie-what.shtml"
                target="_blank"
                title="新手指引"
                onclick="PTTSendClick('gameNav','gameNav-guide','指引')"
              >
                <i class="icon-zhiyin"></i>
                指引
              </a>
              <a
                href="//lol.qq.com/act/djc_qt_rookie/web/a20141205rookie/index.htm"
                target="_blank"
                title="新手礼包"
                onclick="PTTSendClick('gameNav','gameNav-gift','礼包')"
              >
                <i class="icon-gift"></i>
                礼包
              </a>
            </div>
          </li>
          <li class="p2" title="领取中心">
            <a
              class="herf-type-0"
              href="//lol.qq.com/act/a20180929awards/index.html?ADTAG=lolweb.v3#box2"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-Receive','领取中心')"
              >领取中心</a
            >
          </li>
          <li class="p3" title="在线客服">
            <a
              class="herf-type-1"
              href="//kf.qq.com/product/lol.html?pc_scene=web"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-service','在线客服')"
            >
              <i class="icon-kh"></i>在线客服
            </a>
          </li>
          <li class="p3" title="秩序殿堂">
            <a
              class="herf-type-1"
              href="//lol.qq.com/act/a20171108ambient/index.html"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-zhixudiantang','秩序殿堂')"
            >
              <i class="icon-fhcx"></i>秩序殿堂
            </a>
          </li>
          <li class="p3" title="游戏资料">
            <a
              class="herf-type-1"
              href="https://101.qq.com/?ADTAG=cooperation.glzx.web#/page-index/tab-index"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-gamedata','游戏资料')"
            >
              <i class="icon-yxzl"></i>游戏资料
            </a>
          </li>
          <li class="p4" title="峡谷之巅">
            <a
              class="herf-type-1"
              href="//lol.qq.com/act/a20191210super/index.shtml"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-xiagudianfeng','峡谷之巅')"
            >
              <i class="icon-xgzd"></i>峡谷之巅
            </a>
          </li>
          <li class="p3" title="云顶之弈">
            <a
              class="herf-type-1"
              href="//lol.qq.com/tft/#/index"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-tft','云顶之弈')"
            >
              <i class="icon-tft"></i>云顶之弈<b class="icon-new-1"></b>
            </a>
          </li>
          <li class="p3" title="攻略中心">
            <a
              class="herf-type-1"
              href="//101.qq.com/"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-101','攻略中心')"
            >
              <i class="icon-101"></i>攻略中心
            </a>
          </li>
          <li class="p3" title="LOL宇宙">
            <a
              class="herf-type-1"
              href="//yz.lol.qq.com/zh_CN/"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-yz','LOL宇宙')"
            >
              <i class="icon-yz"></i>LOL宇宙
            </a>
          </li>
          <li class="p4" title="微信绑定">
            <a
              class="herf-type-1"
              href="//lol.qq.com/act/a20180607wechatbinding/index.html?primary=qq"
              target="_blank"
              onclick="PTTSendClick('gameNav','gameNav-bindwx','微信绑定')"
            >
              <i class="icon-wxbd"></i>微信绑定
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Carousel from "./Carousel.vue";
import NewsAds from "./NewsAds.vue";
import Activity from "./Activity.vue";

export default {
  components: {
    NewsAds,
    Carousel,
    Activity,
  },
};
</script>

<style scoped>
.g-zoombox {
  width: 100%;
  min-width: 1358px;
  height: auto;
  margin: 0 auto;
}
.g-index-wrap1 {
  width: 1358px;
  height: auto;
  margin: 0 auto;
  padding: 40px 0 80px 0;
  *zoom: 1;
}
/* 游戏功能导航 */
.m-gamefunc-nav {
    width: 496px;
    height: 335px;
    float: right;
    margin-top: 50px;
    position: relative;
}
.slide-nav-ul>li {
    float: left;
    list-style: none;
}
.herf-download {
    float: left;
    width: 366px;
    height: 168px;
    overflow: hidden;
    background-image: url(//game.gtimg.cn/images/lol/v3/pic-download.png);
    -webkit-transition: filter .5s;
    transition: filter .5s;
    filter: brightness(1);
    -webkit-filter: brightness(1);
    position: relative;
}
.herf-download>video {
    display: block;
    width: 366px;
    height: 168px;
}
.herf-mask {
    display: block;
    width: 100%;
    height: 100%;
    position: absolute;
    left: 0;
    top: 0;
    font-size: 0;
}
a {
    text-decoration: none;
}
.m-gamefunc-nav .p1 {
    margin-left: 12px;
}
.btn-flashmen {
    float: left;
    background-position: -193px -316px;
    width: 118px;
    height: 76px;
    color: #fff;
    font-size: 14px;
    font-weight: 700;
    text-align: center;
    line-height: 76px;
    overflow: hidden;
    position: relative;
}
.btn-flashmen .inner-hover {
    display: none;
    position: absolute;
    left: 0;
    top: 0;
    width: 120px;
    height: 100%;
    overflow: hidden;
    background-color: #fff;
}
.btn-flashmen .inner-hover>a {
    float: left;
    width: 60px;
    box-sizing: border-box;
    border-right: 1px #eee solid;
    color: #424242;
    font-size: 12px;
    line-height: 30px;
}
.btn-flashmen .inner-hover>a>i {
    display: block;
    margin: 18px auto 0 auto;
}
.m-gamefunc-nav .p2 {
    margin: 17px 0 0 12px;
}
.herf-type-0 {
    float: left;
    background-position: -193px -316px;
    width: 118px;
    height: 76px;
    color: #fff;
    font-size: 14px;
    font-weight: 700;
    text-align: center;
    line-height: 76px;
    -webkit-transition: filter .5s;
    transition: filter .5s;
    filter: brightness(1);
    -webkit-filter: brightness(1);
}
.m-gamefunc-nav .p3 {
    margin: 15px 16px 0 0;
}
.m-gamefunc-nav .p4 {
    margin: 15px 16px 0 0;
}
.icon-kh, .icon-wjsq {
    margin-top: -4px;
}
</style>