<template>
  <div class="home">
    <HomeHeader/>
  </div>
</template>

<script>
import HomeHeader from './components/Home-header'
export default {
  name: 'Home',
  components: {
    HomeHeader
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
