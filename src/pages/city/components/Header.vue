<template>
  <div class="header">
    城市选择
    <router-link to="/">
      <div class="iconfont header-icon">&#xe624;</div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
  @import "~@/assets/style/varibles.styl"
  .header
    overflow: hidden
    height: @headerHight
    line-height: $headerHight
    text-align: center
    color: #fff
    background: $bgColor
    font-size: .32rem
    position: relative
    .header-icon
      position: absolute
      top: 0
      left: 0
      width: .64rem
      text-align: center
      font-size: .4rem
      color: #fff
</style>
