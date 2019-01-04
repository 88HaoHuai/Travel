<template>
  <div>
    <div class="banner" @click="handleBannerClick">
      <img class="banner-img"
      src="http://img1.qunarzz.com/sight/p0/1712/95/95f38f28a6ff19cba3.img.jpg_600x330_682f736a.jpg" />
      <div class="banner-info">
        <div class="banner-title">水奥雪世界(AAAA景区)</div>
        <div class="banner-number">
          <span class="iconfont banner-icon">&#xe692;</span>
          39
        </div>
      </div>
    </div>
    <common-gallary
    :imgs="imgs"
    v-show="showGallary"
    @close="handleGallaryClose"
    ></common-gallary>
  </div>
</template>

<script>
  import CommonGallary from 'common/gallary/Gallary'
	export default {
		name: 'DetailBanner',
    data () {
      return {
        showGallary: false,
        imgs: ['http://img1.qunarzz.com/sight/p0/1812/36/3681190a5aeb0d79a3.img.jpg_r_800x800_802f0354.jpg', 'http://img1.qunarzz.com/sight/p0/1712/a8/a82aba7c2a07a4c0a3.img.jpg_r_800x800_4717cf28.jpg']
      }
    },
    methods: {
      handleBannerClick () {
        this.showGallary = true
      },
      handleGallaryClose () {
        this.showGallary = false
      }
    },
    components: {
      CommonGallary
    }
	}
</script>

<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    // height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      display: flex
      positon: absolute
      margin-top: -.5rem
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color: #fff
      background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.8))
      .banner-title
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        height: .32rem
        line-height: .32rem
        margin-top: .14rem
        padding: 0 .4rem
        border-radius: .2rem
        background: rgba(0, 0, 0, .8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
