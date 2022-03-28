<template>
  <!-- 官网导航 -->
  <div class="comm-head">
    <div class="head-normal">
      <!-- log图标 -->
      <a class="logo" href="/" title="英雄联盟官网">
        <img
          src="//game.gtimg.cn/images/lol/v3/logo-public.png"
          width="167"
          height="60"
          alt="英雄联盟"
        />
      </a>
      <!-- 官网导航 -->
      <ul class="head-nav"  @mouseover = "Gfocus">
        <li v-for="(n, index) in navigationarray" :key="index" >
          <a
            href="https://101.qq.com/#/page-index/tab-index"
            target="_blank"
            onclick="PTTSendClick('topnav','topnav-0','游戏资料');"
            title="游戏资料"
          >
            <span class="head-nav-title">{{ n.zw }}</span>
            <span class="head-nav-subtitle">{{ n.yw }}</span>
          </a>
        </li>
      </ul>
      <!-- 玩家信息 -->
      <div class="head-userinfo-normal">
        <div class="head-userinfo-avatar">
          <img
            src="//game.gtimg.cn/images/lol/v2/personal/avatar/default.png"
            width="36"
            height="auto"
            alt="玩家头像"
          />
          <span></span>
          <a
            href="//lol.qq.com/space/index.shtml"
            target="_blank"
            class="herf-mask"
            title="个人中心"
          ></a>
        </div>
        <div class="head-userinfo-brief">
          <p class="unlogin">
            亲爱的召唤师，欢迎<a href="javascript:T_Login.login()">登录</a>
          </p>
        </div>
      </div>
      <!-- 掌盟图标 -->
      <span class="head-app-normal">
        <a href="//lol.qq.com/app/index.html" class="comm-icon-phone"></a>
      </span>
      <!-- 搜索按钮 -->
      <a
        class="head-search-btn"
        id="J_headSearchBtn"
        href="javascript:"
        title="搜索"
      >
        <i class="comm-icon-search"></i>
      </a>
    </div>
    <!-- 官网导航子菜单 -->
    <div class="head-nav-sub" :style="{display:hide}"  @mouseleave.stop = "Ofocus">
      <div class="head-nav-sub-inner" >
        <ul id="J_headNavSub">
          <li>
            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-0','游戏下载');"
              href="//lol.qq.com/download.shtml?ADTAG=innercop.lol.web.top"
              target="_blank"
            >
              游戏下载
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-1','新手指引');"
              href="//lol.qq.com/data/newbie-what.shtml"
              target="_blank"
            >
              新手指引
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-2','资料库');"
              href="https://101.qq.com/#/page-index/tab-index"
              target="_blank"
            >
              资料库
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-3','云顶之弈');"
              href="//lol.qq.com/tft/"
              target="_blank"
            >
              <i class="icon-new"></i>
              云顶之弈
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-4','攻略中心');"
              href="//101.qq.com/"
              target="_blank"
            >
              <i class="icon-new"></i>
              攻略中心
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-5','开发者基地');"
              href="//lol.qq.com/nexus/pc/"
              target="_blank"
            >
              开发者基地
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-6','海克斯战利品库');"
              href="//lol.qq.com/act/a20171205hextech/"
              target="_blank"
            >
              海克斯战利品库
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-1-7','英雄联盟宇宙');"
              href="//yz.lol.qq.com/"
              target="_blank"
            >
              英雄联盟宇宙
            </a>
          </li>

          <li>
            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-2-0','点券充值');"
              href="//lol.qq.com/comm-htdocs/pay/new_index.htm?t=lol"
              target="_blank"
            >
              点券充值
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-2-1','道聚城');"
              href="//daoju.qq.com/lol/"
              target="_blank"
            >
              <i class="icon-hot"></i>
              道聚城
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-2-2','周边商城');"
              href="//lolriotmall.qq.com/index.shtml?ADTAG=lol.rk.gw.top&amp;adunionsid=gwtop"
              target="_blank"
            >
              周边商城
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-2-3','LOL桌游');"
              href="//lol.qq.com/act/a20161011mvm/index.htm"
              target="_blank"
            >
              LOL桌游
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-2-4','网吧特权');"
              href="//cafe.qq.com/tpl/lol/index.html"
              target="_blank"
            >
              网吧特权
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-2-5','电竞小说');"
              href="//lol.qq.com/act/a20181124novel/?ADTAG=innercop.lol.web.top"
              target="_blank"
            >
              电竞小说
            </a>
          </li>

          <li>
            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-0','视频中心');"
              href="//lol.qq.com/v/v2/index.shtml"
              target="_blank"
            >
              视频中心
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-1','官方微信');"
              href="//lol.qq.com/act/a20160425wxlol/"
              target="_blank"
            >
              官方微信
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-2','官方微博');"
              href="//weibo.com/lol"
              target="_blank"
            >
              官方微博
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-3','玩家创作馆');"
              href="//tr.lol.qq.com/"
              target="_blank"
            >
              玩家创作馆
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-4','玩家服务');"
              href="//lol.qq.com/act/a20180418yxny/"
              target="_blank"
            >
              玩家服务
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-5','LOL组队专区');"
              href="https://lol.qq.com/act/a20200319clash/index.html?e_code=458230"
              target="_blank"
            >
              <i class="icon-new"></i>
              LOL组队专区
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-6','作者入驻计划');"
              href="https://lol.qq.com/author/#/homepage"
              target="_blank"
            >
              <i class="icon-new"></i>
              作者入驻计划
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-3-7','英雄联盟素材库');"
              href="https://lol.icreate.qq.com/v3"
              target="_blank"
            >
              <i class="icon-new"></i>
              英雄联盟素材库
            </a>
          </li>

          <li>
            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-0','LPL职业联赛');"
              href="https://lpl.qq.com/es/lpl/2022/"
              target="_blank"
            >
              <i class="icon-hot"></i>
              LPL职业联赛
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-1',' LDL发展联赛');"
              href="https://lpl.qq.com/es/ldl/2022/"
              target="_blank"
            >
              LDL发展联赛
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-2','全球总决赛');"
              href="https://lpl.qq.com/es/worlds/2021/"
              target="_blank"
            >
              全球总决赛
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-3','城市英雄争霸赛');"
              href="https://lpl.qq.com/act/a20200707city/index.html"
              target="_blank"
            >
              城市英雄争霸赛
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-4','全明星赛');"
              href="https://lpl.qq.com/act/a20201218allstar/"
              target="_blank"
            >
              全明星赛
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-5','德玛西亚杯');"
              href="https://lpl.qq.com/act/a20211206demacia/index.html"
              target="_blank"
            >
              德玛西亚杯
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-6','全国高校联赛');"
              href="https://lpl.qq.com/act/a20210928lcl/index.html"
              target="_blank"
            >
              全国高校联赛
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-4-7','云顶之弈公开赛');"
              href="https://lpl.qq.com/act/a20210719toc/index.html"
              target="_blank"
            >
              <i class="icon-new"></i>
              云顶之弈公开赛
            </a>
          </li>

          <li>
            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-0','图标自助领取');"
              href="https://lol.qq.com/act/a20210625icon/index.html"
              target="_blank"
            >
              <i class="icon-hot"></i>
              图标自助领取
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-1','转区系统');"
              href="https://lol.qq.com/act/a20200710transferzone/index.html"
              target="_blank"
            >
              <i class="icon-new"></i>
              转区系统
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-2','封号查询');"
              href="/act/a20151118fh/"
              target="_blank"
            >
              <i class="icon-hot"></i>
              封号查询
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-3','账号注销');"
              href="/act/a20200227logout/"
              target="_blank"
            >
              账号注销
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-4','信誉分系统');"
              href="/act/a20190528lolscore/"
              target="_blank"
            >
              <i class="icon-new"></i>
              信誉分系统
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-5','服务器状态查询');"
              href="/act/a20150326dqpd/"
              target="_blank"
            >
              服务器状态查询
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-6','秩序殿堂');"
              href="/act/a20171108ambient/index.html"
              target="_blank"
            >
              秩序殿堂
            </a>

            <a
              class="head-nav-sub-a"
              onclick="PTTSendClick('topnav','topnav-5-7','峡谷之巅');"
              href="/act/a20191210super/index.shtml"
              target="_blank"
            >
              峡谷之巅
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navigationarray: [
        { zw: "游戏资料", yw: "GAME INFO" },
        { zw: "商城/合作", yw: "STORE" },
        { zw: "社区互动", yw: "COMMUNITY" },
        { zw: "赛事官网", yw: "ESPORTS" },
        { zw: "自助系统", yw: "SYSTEM" },
      ],
      hide:"none"
    };
  },
  methods:{
        Gfocus(){
            this.hide = "block"
            console.log("移动了");
        },
        Ofocus(){
          this.hide = "none"
        }
    }
};
</script>

<style  scoped>
.comm-head {
  width: 100%;
  height: 78px;
  overflow: visible;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 11;
}
.head-normal {
  width: 100%;
  max-width: 1358px;
  min-width: 1230px;
  height: 78px;
  margin: 0 auto;
  position: relative;
  z-index: 10;
}
.comm-head .logo {
  float: left;
  width: 132px;
  height: 49px;
  margin-top: 10px;
}
.head-nav {
  width: 55%;
  height: 78px;
  box-sizing: border-box;
  margin-left: 30px;
  padding-top: 16px;
  float: left;
}

.head-nav > li {
  float: left;
  list-style: none;
  width: 20%;
  height: 78px;
  text-align: center;
}
.head-nav-title {
  display: block;
  color: #fff;
  font-size: 18px;
  letter-spacing: 1px;
}
/* 玩家信息 */
.head-userinfo-normal {
  float: right;
  width: 244px;
  height: 78px;
  position: relative;
  z-index: 3;
}
.head-userinfo-avatar {
  float: left;
  width: 48px;
  height: 48px;
  position: relative;
  margin-top: 14px;
  line-height: 48px;
  text-align: center;
  font-size: 0;
}
.head-userinfo-avatar > img {
  display: inline-block;
  vertical-align: middle;
  *zoom: 1;
  *display: inline;
  width: 36px;
  height: auto;
  border-radius: 50%;
}
.head-userinfo-avatar > span {
  display: block;
  background-position: -216px -117px;
  width: 48px;
  height: 48px;
  position: absolute;
  top: 0;
  left: 0;
}
.comm-head a {
  text-decoration: none;
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
.head-userinfo-brief {
  float: left;
  margin-left: 10px;
  height: 78px;
}
.head-userinfo-brief > .logined {
  color: #cdbe91;
  line-height: 78px;
  font-size: 0;
}
.head-userinfo-brief a {
  font-size: 16px;
}
/* 搜索按钮 */

.head-search-btn {
  float: right;
  width: 40px;
  height: 40px;
  text-align: center;
  line-height: 40px;
  margin: 17px 12px 0 0;
}
.head-search-btn > i {
  display: inline-block;
  vertical-align: middle;
}
.comm-icon-search {
  background-position: -381px -39px;
  width: 21px;
  height: 21px;
}

/* 掌盟图标 */
.head-app-normal {
  float: right;
  width: 40px;
  height: 40px;
  text-align: center;
  line-height: 40px;
  margin: 17px 31px 0 0;
}
.head-app-normal > a {
  display: inline-block;
  vertical-align: middle;
}
.comm-icon-phone {
  background-position: -303px -84px;
  width: 16px;
  height: 24px;
}
/* 官网导航子菜单 */


.head-nav-sub {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  overflow: hidden;
  background: url(//game.gtimg.cn/images/lol/v3/dark60-bg-repeat.png) repeat;
  padding: 88px 0 32px 0;
}
.head-nav-sub .head-nav-sub-inner {
  width: 100%;
  max-width: 1358px;
  min-width: 1230px;
  height: auto;
  margin: 0 auto;
}
.head-nav-sub ul {
  width: 55%;
  overflow: hidden;
  margin-left: 161px;
}
.head-nav-sub ul > li {
  list-style: none;
  width: 20%;
  float: left;
  height: auto;
  overflow: visible;
}
.comm-head a {
  text-decoration: none;
}
.head-nav-sub-a {
  display: block;
  width: 100%;
  height: 29px;
  overflow: hidden;
  line-height: 29px;
  color: #e1e1e1;
  font-size: 14px;
  text-align: center;
}
</style>