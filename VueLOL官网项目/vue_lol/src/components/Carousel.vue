<template>
    <!-- 轮播图 -->
    <div class="m-promo" id="J_promo" exposure-tag="indexScroll,首页轮播">
        <ul
          class="promo-img-list"
          id="promoImgList"
          style="width: 4100px;"
         :style="{marginLeft: stlobj+'px'}"
        >
          <li class="promo-item">
            <a
              href="https://daoju.qq.com/lol/list/439-0-0-0-0-0-0-0-0-0-0-00-0-0-1-1.shtml?ADTAG=innercop.lol.SY.shoppinglist_new_439&amp;e_code=500130"
            >
              <img
                src="//ossweb-img.qq.com/upload/adw/image/977/20220222/132b7dea7a8ff48b44abbfc1bbaf4239.jpeg"
                width="820"
                height="340"
                alt="神话级小小英雄"
              />
            </a>
          </li>
          <li class="promo-item">
            <a
              href="https://lol.qq.com/act/a20220121lunarchest/index.html?e_code=500131"
            >
              <img
                src="//ossweb-img.qq.com/upload/adw/image/977/20220223/bf4d1c076c6e039e46f9b723c60c0820.jpeg"
                width="820"
                height="340"
                alt="2022金虎贺岁"
              />
            </a>
          </li>
          <li class="promo-item">
            <a
              href="https://lolm.qq.com/act/a20220107pass/index-pc.html?e_code=500132"
            >
              <img
                src="//ossweb-img.qq.com/upload/adw/image/977/20220225/886862fc05bc377c0e26ed0aa4bf2413.jpeg"
                width="820"
                height="340"
                alt="掌盟夺宝行迹"
              />
            </a>
          </li>
          <li class="promo-item">
            <a href="https://lpl.qq.com/es/lpl/2022/?e_code=500133">
              <img
                src="//ossweb-img.qq.com/upload/adw/image/977/20220227/dcc62626c9112a4dabd5adcff30d7da6.jpeg"
                width="820"
                height="340"
                alt="LPL春季赛"
              />
            </a>
          </li>
          <li class="promo-item">
            <a
              href="https://lol.qq.com/act/a20220218renataglasc/index.html?e_code=500134"
              onclick="PTTSendClick('indexScroll','scroll-22131','新英雄 炼金男爵');"
            >
              <img
                src="//ossweb-img.qq.com/upload/adw/image/977/20220218/a4703b717ccf84b05816af3361e559dc.jpeg"
                width="820"
                height="340"
                alt="新英雄 炼金男爵"
              />
            </a>
          </li>
        </ul>
        <!-- 轮播图底部 -->
        <div class="promo-title-list" id="promoTitleList">
          <span class="title" :class="Selected1" data-bannerid="22029" @mouseover="lb(1)" style="width: 164px"
            >神话级小小英雄</span
          ><span
            class="title"
            :class="Selected2"
            @mouseover="lb(2)"
            data-bannerid="22128"
            style="width: 164px"
            >2022金虎贺岁</span
          ><span class="title" :class="Selected3" data-bannerid="22129" @mouseover="lb(3)" style="width: 164px"
            >掌盟夺宝行迹</span
          ><span class="title" :class="Selected4" data-bannerid="22130" @mouseover="lb(4)" style="width: 164px"
            >LPL春季赛</span
          ><span class="title" :class="Selected5" data-bannerid="22131" @mouseover="lb(5)" style="width: 164px"
            >新英雄 炼金男爵</span
          >
        </div>
        
    </div>
</template>

<script>
export default {
      data(){
      return{
        stlobj:0,
        Selected1:'selected',
        Selected2:'',
        Selected3:'',
        Selected4:'',
        Selected5:'',
       }
      
    },
    // vue完成模板的解析并把初始的真实DOM元素放入页面后（加载完毕） 调用mounted
   mounted(){
      setInterval(() => {
        this.stlobj -= 820
        if (this.stlobj<-3280) {
          this.stlobj = 0;
        }
        switch (this.stlobj) {
          case 0:
            this.Selected1 = 'selected';
            this.Selected2 = '';
            this.Selected3 = '';
            this.Selected4 = '';
            this.Selected5 = '';
               break;
          case -820:
            this.Selected1 = '';
            this.Selected2 = 'selected';
            this.Selected3 = '';
            this.Selected4 = '';
            this.Selected5 = '';
            break;
          case -1640:
            this.Selected1 = '';
            this.Selected2 = '';
            this.Selected3 = 'selected';
            this.Selected4 = '';
            this.Selected5 = '';
            break;
          case -2460:
            this.Selected1 = '';
            this.Selected2 = '';
            this.Selected3 = '';
            this.Selected4 = 'selected';
            this.Selected5 = '';
            break;
          case -3280:
            this.Selected1 = '';
            this.Selected2 = '';
            this.Selected3 = '';
            this.Selected4 = '';
            this.Selected5 = 'selected';
            break;
        
        }
      }, 3000)
      
   },
   methods:{
     lb(a){
         switch (a) {
          case 1:
            this.stlobj = 0;
            this.Selected1 = 'selected';
            this.Selected2 = '';
            this.Selected3 = '';
            this.Selected4 = '';
            this.Selected5 = '';
               break;
          case 2:
            this.stlobj = -820;
            this.Selected1 = '';
            this.Selected2 = 'selected';
            this.Selected3 = '';
            this.Selected4 = '';
            this.Selected5 = '';
            break;
          case 3:
            this.stlobj = -1640;
            this.Selected1 = '';
            this.Selected2 = '';
            this.Selected3 = 'selected';
            this.Selected4 = '';
            this.Selected5 = '';
            break;
          case 4:
             this.stlobj = -2460;
            this.Selected1 = '';
            this.Selected2 = '';
            this.Selected3 = '';
            this.Selected4 = 'selected';
            this.Selected5 = '';
            break;
          case 5:
            this.stlobj = -3280;
            this.Selected1 = '';
            this.Selected2 = '';
            this.Selected3 = '';
            this.Selected4 = '';
            this.Selected5 = 'selected';
            break;
        
        }
     }
   }
}
</script>

<style scoped>
.m-promo {
  float: left;
  width: 820px;
  height: 380px;
  overflow: hidden;
  background-color: #e3e2e2;
  position: relative;
}
.promo-img-list {
  width: auto;
  height: 340px;
  overflow: hidden;
  position: relative;
}
.promo-img-list > li {
  list-style: none;
  float: left;
  width: 820px;
  height: 340px;
  overflow: hidden;
}
.promo-title-list>span {
    list-style: none;
    float: left;
    width: 164px;
    height: 40px;
    box-sizing: border-box;
    background-color: #e3e2e2;
    font-size: 14px;
    text-align: center;
    line-height: 40px;
    color: #424242;
    letter-spacing: 1px;
}
.promo-title-list>span.selected {
    color: #ab8e66;
    background-color: #f7f6f6;
    border-bottom: 2px #cea861 solid;
}
</style>