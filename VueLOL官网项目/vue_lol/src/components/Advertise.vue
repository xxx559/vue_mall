<template>
  <div class="comm-topact" :class="ys" exposure-tag="topact,头部广告">
    <img
      class="topact-big-img"
      
      src="https://img.crawler.qq.com/lolwebschool/0/JAutoCMS_LOLWeb_67a9495406efe50d101de57734f67845/0"
    />
    <img
      class="topact-small-img"
      src="https://img.crawler.qq.com/lolwebschool/0/JAutoCMS_LOLWeb_78557b30a56986764f18ee16d9bff298/0"
    />
    <div class="act-fullscreen-mask"></div>
    <div class="dark-mask"></div>
   
  </div>
</template>

<script>
import pubsub from 'pubsub-js'
export default {
  data(){
       return{
            ys:"big"
       } 
    },
   mounted(){
     this.pubId = pubsub.subscribe('gd',(msgName,data) => {
       this.ys = data
     })
   },
   beforDestroy() {
      pubsub.unsubscribe(this.pubId)
  },
};
</script>

<style scoped>
.comm-topact.big {
  height: 720px !important;
}
.comm-topact {
  width: 100%;
  min-width: 1230px;
  height: 360px;
  overflow: hidden;
  position: relative;
  background: center top no-repeat;
  -webkit-transition: height 0.6s, background, 0.6s;
  transition: height 0.6s, background, 0.6s;
}

.comm-topact.big .topact-big-img {
  z-index: 1;
}
.comm-topact.big .topact-small-img {
  opacity: 0;
}
.topact-small-img {
  -webkit-transition: opacity 0.6s;
  transition: opacity 0.6s;
  opacity: 1;
}
.comm-topact .dark-mask {
  width: 100%;
  height: 131px;
  position: absolute;
  left: 0;
  top: 0;
  background: url(//game.gtimg.cn/images/lol/v3/dark-jianbian-repeatx-0.png)
    repeat center top;
  z-index: 1;
}
</style>