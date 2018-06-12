<template>
  <div class="header">
    <div class="left">
      <div class="iconfont icon-back">&#xe602;</div>
    </div>
    <div class="center">
      <span class="iconfont">&#xe6a4;</span>
      <span class="center-line">输入城市/景点/游玩主题</span>
    </div>
    <div class="right">
      城市
      <span class="iconfont icon-arrow">&#xe6a5;</span>
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
      border-radius: .06rem
      margin-top: .14rem
      margin-left: .16rem
      line-height: .56rem
      height: .6rem
      padding-left: .2rem
      color: #e4e7ea
      .center-line
        margin-left: .02rem
    .right
      width: 1.32rem
      float: right
      line-height: .88rem
      text-align: center
      .icon-arrow
        font-size: .24rem
        margin-left: -.04rem
</style>
