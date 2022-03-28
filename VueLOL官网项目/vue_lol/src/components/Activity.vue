<template>
  <div class="m-act">
    <!-- 活动导航 -->
    <div class="part-top-tab">
      <h2><span>丨</span> 热门活动</h2>
      <ul class="part-tab-title">
        <li @mouseover="toggleUl(1)" class="">正在进行</li>
        <li @mouseover="toggleUl(2)" class="">商城特惠</li>
        <li @mouseover="toggleUl(3)" class="selected">长期活动</li>
      </ul>
    </div>
    <!-- 活动内容1 -->
    <div class="m-act-list" :style="{display: divys[0].divys}">
      <ul id="J_actListContainer">
        <li class="act-item" @mouseover="ShowContent(1)" @mouseleave="ShowContent1">
          <img
            src="//ossweb-img.qq.com/images/clientpop/act/lol_1646720450_uploadnewsImg.jpg"
            alt="运动 舞蹈 琦琦全都会"
            width="193"
            height="207"
          />
          <p>运动 舞蹈 琦琦全都会</p>

          <a class="overtime">78天后结束</a>

          <i class="icon-new-1"></i>

          <div class="innerhover-border"  :style="{display: disp[0].disp}">
            <i class="hover-border-1"></i>
            <div class="innerhover-border-inner">
              <h4 class="p1">运动 舞蹈 琦琦全都会</h4>
              <p class="p2">海克斯冠军杯登顶同款小小英雄</p>

              <p class="p2">2022-03-08 - 2022-05-25</p>
            </div>
          </div>
          <a
            class="herf-mask"
            href="https://daoju.qq.com/lol/list/439-0-0-0-0-0-0-0-0-0-0-00-0-0-1-1.shtml?ADTAG=innercop.lol.SY.shoppinglist_new_439&amp;e_code=524631"
            target="_blank"
            title="运动 舞蹈 琦琦全都会"
            onclick="PTTSendClick('act','act-13421','运动 舞蹈 琦琦全都会')"
          ></a>
        </li>

        <li class="act-item" @mouseover="ShowContent(2)" @mouseleave="ShowContent1">
          <img
            src="//ossweb-img.qq.com/images/clientpop/act/lol_1646383076_uploadnewsImg.jpg"
            alt="小蜜蜂宝典Ⅱ"
            width="193"
            height="207"
          />
          <p>小蜜蜂宝典Ⅱ</p>

          <a class="overtime">22天后结束</a>

          <i class="icon-new-1"></i>

          <div class="innerhover-border" :style="{display: disp[1].disp}">
            <i class="hover-border-1"></i>
            <div class="innerhover-border-inner">
              <h4 class="p1">小蜜蜂宝典Ⅱ</h4>
              <p class="p2">
                解锁宝典赢取丰富奖励 有机会获得18-19年至臻皮肤典藏版
              </p>

              <p class="p2">2022-03-04 - 2022-03-30</p>
            </div>
          </div>
          <a
            class="herf-mask"
            href="https://lol.qq.com/act/a20220302bee/index.html?e_code=528424"
            target="_blank"
            title="小蜜蜂宝典Ⅱ"
            onclick="PTTSendClick('act','act-13414','小蜜蜂宝典Ⅱ')"
          ></a>
        </li>

        <li class="act-item" @mouseover="ShowContent(3)" @mouseleave="ShowContent1">
          <img
            src="//ossweb-img.qq.com/images/clientpop/act/lol_1646362205_uploadnewsImg.jpg"
            alt="2022小蜜蜂"
            width="193"
            height="207"
          />
          <p>2022小蜜蜂</p>

          <a class="overtime">23天后结束</a>

          <i class="icon-new-1"></i>

          <div class="innerhover-border" :style="{display: disp[2].disp}">
            <i class="hover-border-1"></i>
            <div class="innerhover-border-inner">
              <h4 class="p1">2022小蜜蜂</h4>
              <p class="p2">春风得意 甜蜜出击</p>

              <p class="p2">2022-03-04 - 2022-03-31</p>
            </div>
          </div>
          <a
            class="herf-mask"
            href="https://lol.qq.com/act/a20220304beekeeper/index.html?e_code=528419"
            target="_blank"
            title="2022小蜜蜂"
            onclick="PTTSendClick('act','act-13412','2022小蜜蜂')"
          ></a>
        </li>

        <li class="act-item" @mouseover="ShowContent(4)" @mouseleave="ShowContent1">
          <img
            src="//ossweb-img.qq.com/images/clientpop/act/lol_1646107471_uploadnewsImg.jpg"
            alt="2022电玩秘宝"
            width="193"
            height="207"
          />
          <p>2022电玩秘宝</p>

          <a class="overtime">22天后结束</a>

          <div class="innerhover-border" :style="{display: disp[3].disp}">
            <i class="hover-border-1"></i>
            <div class="innerhover-border-inner">
              <h4 class="p1">2022电玩秘宝</h4>
              <p class="p2">钻石宝箱优先未解锁 登录即赠体验券</p>

              <p class="p2">2022-03-01 - 2022-03-30</p>
            </div>
          </div>
          <a
            class="herf-mask"
            href="https://lol.qq.com/act/a20220301arcadechest/index.html?e_code=528338"
            target="_blank"
            title="2022电玩秘宝"
            onclick="PTTSendClick('act','act-13399','2022电玩秘宝')"
          ></a>
        </li>
      </ul>
    </div>
    <!-- 活动内容2 -->
    <div class="m-act-list" :style="{display: divys[1].divys}">
        <ul id="J_actListContainer">
          <li class="act-item"  @mouseover="ShowContent(1)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1645165128_uploadnewsImg.jpg" alt="洛与霞雕塑预售开启" width="193" height="207">
            <p>洛与霞雕塑预售开启</p>
            
            <a class="overtime">83天后结束</a>
            
            
            <div class="innerhover-border" :style="{display: disp[0].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">洛与霞雕塑预售开启</h4>
                <p class="p2">预定专属周边福利赠品！</p>
                
                <p class="p2">2022-02-14 - 2022-05-31</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lolriotmall.qq.com/act/a20220214luoxia/index.html?ADTAG=lolriotmall.pc.lolhdzx.ad&amp;e_code=528128" target="_blank" title="洛与霞雕塑预售开启" onclick="PTTSendClick('act','act-13349','洛与霞雕塑预售开启')"></a>
          </li>
          
          <li class="act-item"  @mouseover="ShowContent(2)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1646045394_uploadnewsImg.jpg" alt="星之守护者佐伊雕塑预售" width="193" height="207">
            <p>星之守护者佐伊雕塑预售</p>
            
            <a class="overtime">长期活动</a>
            
            
            <div class="innerhover-border" :style="{display: disp[1].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">星之守护者佐伊雕塑预售</h4>
                <p class="p2">周边预定专属礼 买赠图标道具</p>
                
                <p class="p2">开启时间: 2022-02-28</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lolriotmall.qq.com/detail.shtml?id=22340&amp;ADTAG=lolriotmall.pc.lolhdzx.ad&amp;e_code=481128" target="_blank" title="星之守护者佐伊雕塑预售" onclick="PTTSendClick('act','act-13393','星之守护者佐伊雕塑预售')"></a>
          </li>
          
          <li class="act-item"  @mouseover="ShowContent(3)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1641269390_uploadnewsImg.jpg" alt="约德尔人手办盲盒" width="193" height="207">
            <p>约德尔人手办盲盒</p>
            
            <a class="overtime">长期活动</a>
            
            
            <div class="innerhover-border" :style="{display: disp[2].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">约德尔人手办盲盒</h4>
                <p class="p2">小英雄，大梦想！约德尔人潮玩手办盲盒登场！</p>
                
                <p class="p2">开启时间: 2021-12-10</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lolriotmall.qq.com/act/a20211210yordles/index.html?e_code=526761" target="_blank" title="约德尔人手办盲盒" onclick="PTTSendClick('act','act-13213','约德尔人手办盲盒')"></a>
          </li>
          
          <li class="act-item"  @mouseover="ShowContent(4)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1645426311_uploadnewsImg.jpg" alt="魄罗新品系列XL手办 甜蜜登场" width="193" height="207">
            <p>魄罗新品系列XL手办 甜蜜登场</p>
            
            <a class="overtime">已结束</a>
            
            
            
            <div class="innerhover-border"  :style="{display: disp[3].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">魄罗新品系列XL手办 甜蜜登场</h4>
                <p class="p2">甜心魄罗买赠道具 真爱回馈限时开启</p>
                
                <p class="p2">2022-01-27 - 2022-02-28</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lolriotmall.qq.com/act/a20220127poro/index.html?e_code=527749" target="_blank" title="魄罗新品系列XL手办 甜蜜登场" onclick="PTTSendClick('act','act-13312','魄罗新品系列XL手办 甜蜜登场')"></a>
          </li>
          </ul>
       
      </div>
    <!-- 活动内容3 -->
    <div class="m-act-list" :style="{display: divys[2].divys}">
        <ul id="J_actListContainer">
          <li class="act-item"  @mouseover="ShowContent(1)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1646650437_uploadnewsImg.jpg" alt="联名雕塑 限时预售中" width="193" height="207">
            <p>联名雕塑 限时预售中</p>
            
            <a class="overtime">长期活动</a>
            
            
            <i class="icon-new-1"></i>
            
            <div class="innerhover-border"  :style="{display: disp[0].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">联名雕塑 限时预售中</h4>
                <p class="p2">联名雕塑 限时预售中</p>
                
                <p class="p2">开启时间: 2022-03-07</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lolriotmall.qq.com/list.shtml?tagid=458&amp;ADTAG=lolriotmall.pc.lolgw.ad&amp;e_code=522753" target="_blank" title="联名雕塑 限时预售中" onclick="PTTSendClick('act','act-13420','联名雕塑 限时预售中')"></a>
          </li>
          
          <li class="act-item"  @mouseover="ShowContent(2)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1645502463_uploadnewsImg.jpg" alt="神话级小小英雄" width="193" height="207">
            <p>神话级小小英雄</p>
            
            <a class="overtime">长期活动</a>
            
            
            <div class="innerhover-border" :style="{display: disp[1].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">神话级小小英雄</h4>
                <p class="p2">神话级小小英雄来了！源计划 菜大师可通过购买霓虹之夜稀有蛋开启解锁</p>
                
                <p class="p2">开启时间: 2022-02-22</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://daoju.qq.com/lol/list/439-0-0-0-0-0-0-0-0-0-0-00-0-0-1-1.shtml?ADTAG=innercop.lol.SY.shoppinglist_new_439&amp;e_code=524631" target="_blank" title="神话级小小英雄" onclick="PTTSendClick('act','act-13376','神话级小小英雄')"></a>
          </li>
          
          <li class="act-item"  @mouseover="ShowContent(3)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1640317587_uploadnewsImg.jpg" alt="英雄联盟排位FAQ" width="193" height="207">
            <p>英雄联盟排位FAQ</p>
            
            <a class="overtime">长期活动</a>
            
            
            <div class="innerhover-border"  :style="{display: disp[2].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">英雄联盟排位FAQ</h4>
                <p class="p2">了解排位赛上分的一切</p>
                
                <p class="p2">开启时间: 2021-12-24</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lol.qq.com/act/a20211213faq/index.html?e_code=526871" target="_blank" title="英雄联盟排位FAQ" onclick="PTTSendClick('act','act-13187','英雄联盟排位FAQ')"></a>
          </li>
          
          <li class="act-item"  @mouseover="ShowContent(4)" @mouseleave="ShowContent1">
            <img src="//ossweb-img.qq.com/images/clientpop/act/lol_1637216646_uploadnewsImg.jpg" alt="EDG夺冠纪念图标表情领取" width="193" height="207">
            <p>EDG夺冠纪念图标表情领取</p>
            
            <a class="overtime">长期活动</a>
            
            
            <div class="innerhover-border"  :style="{display: disp[3].disp}">
              <i class="hover-border-1"></i>
              <div class="innerhover-border-inner">
                <h4 class="p1">EDG夺冠纪念图标表情领取</h4>
                <p class="p2">在游戏中赢得对局领取纪念图标表情</p>
                
                <p class="p2">开启时间: 2021-11-11</p>
                
              </div>
            </div>
            <a class="herf-mask" href="https://lol.qq.com/act/a20211112champion/souvenir.html?e_code=526006" target="_blank" title="EDG夺冠纪念图标表情领取" onclick="PTTSendClick('act','act-13043','EDG夺冠纪念图标表情领取')"></a>
          </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    data(){
        return {
          disp:[
              {dispId:1,disp:"none"},
              {dispId:2,disp:"none"},
              {dispId:3,disp:"none"},
              {dispId:4,disp:"none"},
            ],
          divys:[
              {divysId:1,divys:"block"},
              {divysId:2,divys:"none"},
              {divysId:3,divys:"none"},
          ]
        }
    },
    methods:{
      ShowContent(toggleid){
        this.disp.forEach((dsp,index) => {
          if (toggleid===dsp.dispId) {
            this.disp[index].disp = "block";
          }else{
            this.disp[index].disp = "none"
          }
        });
      },
      ShowContent1(){
        this.disp.forEach((dsp,index) => {
          this.disp[index].disp = "none";
        });
      },
      toggleUl(toggleid){
        this.divys.forEach((divys,index) => {
           if (toggleid===divys.divysId) {
              this.divys[index].divys = "block";
           }else{
               this.divys[index].divys = "none"
            }
        });
      }
    }
};
</script>

<style scoped>
    .m-act {
    width: 820px;
    height: 335px;
    float: left;
    margin-top: 50px;
    }
    .part-top-tab {
    width: 100%;
    height: 35px;
    position: relative; /* 相对定位 */
    }
    .part-top-tab > h2 {
    position: absolute; /*绝对定位脱离文档流 */
    font-size: 20px;
    vertical-align: middle;
    line-height: 35px;
    width: auto;
    }
    .part-top-tab > h2 > span {
    color: #1da6ba;
    font-weight: bold;
    font-size: 25px;
    }
    .m-act-list {
    width: 100%;
    height: 300px;
    margin-top: 21px;
    }
    .part-tab-title {
    position: absolute;
    width: 692px;
    height: 35px;
    left: 128px;
    border-bottom: 1px #e0e2e2 solid;
    }
    .part-tab-title > li {
    position: relative;
    list-style: none;
    cursor: pointer; /* 鼠标样式 */
    float: left;
    width: auto;
    height: 37px;
    color: #676767;
    font-size: 18px;
    text-align: center;
    line-height: 35px;
    margin-right: 40px;
    }

    .m-act-list>ul {
        width: 840px;
        height: 278px;
        position: relative;
    }
    .m-act-list .act-item {
        margin: 0;
        margin-right: 16px;
    }
    .act-item {
        list-style: none;
        float: left;
        width: 193px;
        height: 278px;
        margin: 0 29px 20px 0;
        overflow: hidden;
        position: relative;
        -webkit-transition: transform .3s;
        transition: transform .3s;
        -webkit-transform: translateY(0);
        transform: translateY(0);
        background-color: #fefefe;
        -webkit-transition:height 10s,transform 2s; /* Safari */
    }
    .act-item:hover {
      margin-top: -10px;
    }
    .act-item>img {
        display: block;
        width: 193px;
        height: 207px;
    }
    img {
        border: 0;
    }
    .act-item>p {
        width: 100%;
        overflow: hidden;
        box-sizing: border-box;
        padding: 6px 10px 4px 10px;
        font-size: 14px;
        color: #424242;
        line-height: 18px;
        text-align: left;
    }
    .act-item>.overtime {
        position: absolute;
        font-size: 12px;
        color: #1da6ba;
        left: 10px;
        bottom: 6px;
    }
    a {
        text-decoration: none;
    }
    .act-item>.icon-hot-1, .act-item>.icon-new-1 {
        position: absolute;
        right: 10px;
        bottom: 8px;
    }
    .icon-hot-1, .icon-new-1 {
        display: inline-block;
        vertical-align: middle;
        *zoom: 1;
        *display: inline;
    }
    .icon-new-1 {
        background-position: -301px -46px;
        width: 29px;
        height: 14px;
    }
    .act-item>.innerhover-border {
        background: url(//game.gtimg.cn/images/lol/v3/dark70-bg-repeat.png) repeat;
        display: none;
        width: 193px;
        height: 207px;
        line-height: 207px;
        position: absolute;
        top: 0;
        left: 0;
        text-align: center;
    }
    .innerhover-border {
        background: url(//game.gtimg.cn/images/lol/v3/dark70-bg-repeat.png) repeat;
        position: absolute;
        top: 0;
        left: 0;
        text-align: center;
    }
    .act-item>.innerhover-border .hover-border-1 {
        display: block;
        position: absolute;
        left: 50%;
        margin-left: -94px;
        top: 50%;
        margin-top: -100px;
        background-position: 0 0;
        width: 188px;
        height: 200px;
    }
    .act-item>.innerhover-border .innerhover-border-inner {
        display: inline-block;
        vertical-align: middle;
        *zoom: 1;
        *display: inline;
        position: relative;
        line-height: 1.5;
        padding: 0 10px;
    }
    .innerhover-border .innerhover-border-inner {
        display: inline-block;
        vertical-align: middle;
        *zoom: 1;
        *display: inline;
        position: relative;
        line-height: 1.5;
        box-sizing: border-box;
        padding: 0 10px;
    }
    .act-item>.innerhover-border .p1 {
        font-size: 16px;
        font-weight: 400;
        color: #cdbe91;
    }
    .innerhover-border .p1 {
        font-size: 16px;
        font-weight: 400;
        color: #cdbe91;
        margin-bottom: 2px;
    }
    .act-item>.innerhover-border .p2 {
        font-size: 12px;
        color: #9d9c9c;
        max-height: 73px;
        overflow: hidden;
    }
    .innerhover-border .p2 {
        overflow: hidden;
        font-size: 12px;
        color: #9d9c9c;
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
</style>