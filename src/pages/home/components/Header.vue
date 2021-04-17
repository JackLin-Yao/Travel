<template>
  <div class="header">
    <div class="header-left"><div class="iconfont back-icon">&#xe624;</div></div>
    <div class="header-input"><span class="iconfont">&#xe632;</span>输入城市/景点/游玩/主题</div>
    <div class="header-right">城市<span class="iconfont arrow-icon">&#xe6aa;</span></div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
  @import '~style/varibles.styl'
  .header
    background: $bgColor
    color: #fff
    line-height: 0.89rem
    display: flex
    .header-left
      width: .70rem
      float: left
      .back-icon
        text-align: center
        font-size: .35rem
    .header-right
      float:right
      width: 1.4rem
      text-align : center
      .arrow-icon
        font-size: .3rem
        margin-left: 0.05rem
    .header-input
      flex: 1
      background: #fff
      height: .63rem
      line-height: .60rem
      border-radius: .1rem
      margin-top: .13rem
      margin-left: .2rem;
      color: #ccc
      padding-left: .2rem;
</style>
