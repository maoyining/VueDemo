<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img :src="item.imgUrl" alt="" class="item-img">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
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
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/cc/19733fc0135062788140cbb48ae606a7.water.jpg_200x200_d9ebe2fd.jpg',
        title: '北京野生动物园',
        desc: '北京野生动物园，带你领略别样的大自然'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/cc/19733fc0135062788140cbb48ae606a7.water.jpg_200x200_d9ebe2fd.jpg',
        title: '北京野生动物园',
        desc: '北京野生动物园，带你领略别样的大自然'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/cc/19733fc0135062788140cbb48ae606a7.water.jpg_200x200_d9ebe2fd.jpg',
        title: '北京野生动物园',
        desc: '北京野生动物园，带你领略别样的大自然'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/cc/19733fc0135062788140cbb48ae606a7.water.jpg_200x200_d9ebe2fd.jpg',
        title: '北京野生动物园',
        desc: '北京野生动物园，带你领略别样的大自然'
      }]
    }
  }
}
</script>
<style lang="stylus" scoped>
@import '~styles/mixins.styl'
  .title
    line-height: .8rem
    text-indent: .2rem
    background :#eee
  .item
    display:flex
    height 1.9rem
    overflow: hidden
    .item-img
      width:1.7rem
      height 1.7rem
      padding:.1rem
  .item-info
    flex:1
    padding:.1rem
    min-width:0 /*小技巧 */
    .item-title
      line-height :.54rem
      font-size:.32rem
      ellipsis()
    .item-desc
      line-height: .4rem
      color:#ccc
      ellipsis()
    .item-button
      margin-top:.2rem
      background :#ff9300
      padding:0 .2rem
      border-radius:.06rem
      color:#fff
</style>
