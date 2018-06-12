<template>
  <div class="home">
    <HomeHeader/>
    <HomeSwiper/>
  </div>
</template>

<script>
import HomeHeader from './components/Home-header'
import HomeSwiper from './components/Home-swiper'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper
  },
  data () {
    return {
      'title': 'BlackXu'
    }
  }
}
</script>

<style>

</style>
