<template>
  <div class="header">
    <div class="header-left">
      <span class="iconfont">&#xe624;</span>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont">&#xe637;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display:flex
    line-height:.86rem
    background: $bgColor
    color:#fff
    .header-left
      width: 0.64rem
      float:left
      text-align :center
    .header-input
      flex:1
      background :#fff
      border-radius:.1rem
      line-height:.64rem
      height:.64rem
      margin-top:.12rem
      margin-left:.2rem
      color:#ccc
      text-align :center
    .header-right
      width:1.24rem
      float:right
      text-align :center
</style>
