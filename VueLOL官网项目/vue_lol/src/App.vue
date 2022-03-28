<template>
  <div id="app">
      <navigtion></navigtion>
      <Advertise></Advertise>
      <ContentSection></ContentSection>
  </div>
</template>

<script>
import pubsub from 'pubsub-js'
import navigtion from './components/navigation.vue'
import Advertise from './components/Advertise.vue'
import ContentSection from './components/ContentSection.vue'
export default {
  name: 'App',
    mounted() {
       window.addEventListener('scroll', this.windowScroll)
    },
    methods:{
      windowScroll() {
        this.pubId =   pubsub.publish('gd','')
      }
    },
    beforDestroy() {
      pubsub.unsubscribe(this.pubId)
    },
  components: {
    navigtion,
    Advertise,
    ContentSection
  }
}
</script>

<style>
  *{
     margin: 0;
     padding: 0;
  }
</style>
