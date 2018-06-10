<template>
  <div class="header">
    <div class="left">
      <div class="iconfont icon-back">&#xe624;</div>
    </div>
    <div class="center">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="right">
      城市
      <span class="iconfont icon-arrow">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home-header'
}
</script>

<style lang="stylus" scoped>
@import '~style/varibles.styl'
  .header
    line-height: .86rem
    display: flex
    background: $bgColor
    color: #fff
    .left
      width: .64rem
      float: left
      .icon-back
        text-align: center
        font-size: .4rem
    .center
      flex: 1
      background: #fff
      border-radius: .1rem
      margin-top: .12rem
      margin-left: .2rem
      line-height: .64rem
      height: .64rem
      padding-left: .2rem
      color: #ccc
    .right
      width: 1.24rem
      float: right
      text-align: center
      .icon-arrow
        font-size: .24rem
        margin-left: -.04rem
</style>
