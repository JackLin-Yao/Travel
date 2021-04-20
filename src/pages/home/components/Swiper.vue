<template>
<div class="wrapper">
  <swiper  :options="swiperOptions">
    <swiper-slide v-for="item of swiperList" :key="item.id">
      <img  class="swiper-img"  :src="item.imgUrl"></swiper-slide>
    <!-- <swiper-slide v-for="item of swiperList" :key="item.id">
      <img  class="swiper-img"  :src="item.imgUrl"></swiper-slide>
    <swiper-slide v-for="item of swiperList" :key="item.id"
    ><img class="swiper-img" :src="item.imgUrl" alt=""></swiper-slide>
    <swiper-slide v-for="item of swiperList" :key="item.id">
      <img class="swiper-img" :src="item.imgUrl"></swiper-slide> -->
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOptions: {
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        },

        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://img1.qunarzz.com/qs/2103/22/dfd49774c7a1f102.jpg'
      },
      {
        id: '0002',
        imgUrl: 'https://img1.qunarzz.com/qs/2103/de/7c7e2cdf695f2602.jpg'
      },

      {
        id: '0003',
        imgUrl: 'https://img1.qunarzz.com/qs/2101/87/f3fa48c8346dab02.jpg'
      },
      {
        id: '0004',
        imgUrl: 'https://img1.qunarzz.com/qs/2101/b5/945dfe4ce22d2302.jpg'
      }
      ]
    }
  }
}
</script>

 <style lang="stylus" scoped>
  // .wrapper
  //   width: 100%
  //   height: 0;
  //   overflow:hidden
  //   .swiper-img
  //     width: 100%
  ..wrapper >>> .swiper-pagination-bullet-active
      background-color : #fff
  .wrapper
    width: 100%;
    height: 0;
    overflow : hidden
    padding-bottom : 40.25%
    background-color : #eee
    .swiper-img
      width: 100%;
 </style>
