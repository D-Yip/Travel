<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of list" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-btn">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      list: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/07/30b534b0de51ccac2906bcb6ba159988.jpg_200x200_2f08733b.jpg',
        title: '长隆野生动物世界',
        desc: '一个值得去的地方，真的是超级棒'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1603/3c/3c514c20a740128b90.water.jpg_200x200_c7102a23.jpg',
        title: '南沙百万葵园',
        desc: '一个值得去的地方，真的是超级棒'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1410/20/41d723daadc98045fe6b7283ba0af40c.jpg_200x200_5a05d5bc.jpg',
        title: '碧水湾温泉度假村',
        desc: '非常棒'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1411/31/74eabd4dc95afd494d92a5006c9ad4f5.water.jpg_200x200_b27fe752.jpg',
        title: '美林湖温泉',
        desc: '美丽温泉'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~@/assets/style/mixins.styl"
  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background-color: #eee
    text-indent: .2rem
  .item
    display: flex
    height: 1.9rem
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-btn
        line-height: .44rem
        margin-top: .16rem;
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
</style>
