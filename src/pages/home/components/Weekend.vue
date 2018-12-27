<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" />
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
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
          imgUrl: 'http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg',
          title: '水奥雪世界',
          desc: '水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界'
        },
        {
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg',
          title: '水奥雪世界',
          desc: '水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界'
        },
        {
          id: '0003',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg',
          title: '水奥雪世界',
          desc: '水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界水奥雪世界，你的世界'
        }]
      }
    }
	}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-index: .2rem
  .item-img-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 33.9%
    .item-img
      width: 100%
  .item-info
    padding: .1rem
    .item-title
      line-height: .54rem
      font-size: .32rem
      ellipsis()
    .item-desc
      line-height: .4rem
      color: #eee
      ellipsis()
</style>
