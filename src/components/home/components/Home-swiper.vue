<template>
  <div class="home-swiper">
    <swiper :options="swiperOption">
      <swiper-slide v-for='item of swiperList' :key='item.id'>
        <img :src="item.imgUrl" class="swiper-img">
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/f2/91b285a08ee21c02.jpg_750x200_8a73fd08.jpg'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1806/fc/e47aa3e1c67bbc02.jpg_750x200_0f3eecf8.jpg'
      }]
    }
  }
}
</script>

<style scoped lang='stylus'>
  .home-swiper >>> .swiper-pagination-bullet-active
    background-color: #fff !important
  .home-swiper
    width: 100%
    height: 26.67vw
    background-color: #eee
    .swiper-img
      width: 100%
</style>
