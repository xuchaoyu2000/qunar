<template>
  <div class="home">
    <HomeHeader/>
    <HomeSwiper/>
    <HomeIcons/>
  </div>
</template>

<script>
import HomeHeader from './components/Home-header'
import HomeSwiper from './components/Home-swiper'
import HomeIcons from './components/Home-icons'

import axios from 'axios'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcons
  },
  data () {
    return {
      'title': 'BlackXu'
    }
  },
  mounted () {
    this.getHomeInfo()
  },
  methods: {
    getHomeInfo () {
      axios.get('/api/index.json')
        .then(this.getHomeInfoSucc)
    },
    getHomeInfoSucc (res) {
      res = res.data
      if (res.ret && res.data) {
        const data = res.data
        console.log(data)
      }
    }
  }
}
</script>

<style>

</style>
