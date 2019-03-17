<template>
  <div class="icons">
    <div class="icon" v-for="item of list" :key="item.id">
      <div class="icon-img">
        <img class="icon-img-content" :src="item.imgUrl"/>
      </div>
      <p class="icon-desc">{{item.name}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      list: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        name: '景点门票'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
        name: '广州必游'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/76/eb88861d78fb9902.png',
        name: '动植物园'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/96/c70f1e85ae4a4f02.png',
        name: '自然风光'
      }, {
        id: '0005',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
        name: '珠江夜游'
      }, {
        id: '0006',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ab/6f7d6e44963c9302.png',
        name: '泡温泉'
      }, {
        id: '0007',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
        name: '一日游'
      }, {
        id: '0008',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/b1/528a9e80403b8c02.png',
        name: '长隆度假区'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~@/assets/style/varibles.styl"
  @import "~@/assets/style/mixins.styl"
  .icons
    overflow: hidden
    height:0
    padding-bottom: 50%
    /*background-color: green;*/
    .icon
      position: relative
      overflow: hidden
      float: left
      width: 25%
      height: 0
      padding-bottom: 25%
      /*background-color: red;*/
      .icon-img
        position: absolute
        top: 0
        left: 0
        right: 0
        bottom: .44rem
        /*background-color: blue;*/
        .icon-img-content
          height: 100%
          display: block
          margin: 0 auto
      .icon-desc
        position: absolute
        left: 0
        right: 0
        bottom: 0
        height: .44rem
        line-height: .44rem;
        color: $darkTextColor
        text-align: center
        ellipsis()
</style>
