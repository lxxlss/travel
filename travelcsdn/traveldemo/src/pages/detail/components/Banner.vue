<template>
 <div>
  <div class="banner" @click="handleBannerClick">
  	<img class="banner-img" src="http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_600x330_bf9c4904.jpg">
  	<div class="banner-info">
  	  <div class="banner-tittle">大连圣亚海洋世界(AAAA景区)</div>
  	  <div class="banner-number"><span class="iconfont banner-icon">&#xe626;</span>39</div>
  	</div>
  </div>
  <fade-animation>
   <common-gallary 
     :imgs="imgs" 
     v-show="showGallary"
     @close="hanleGallaryClose">
    </common-gallary>
  </fade-animation>
 </div>
</template>

<script> 
import FadeAnimation from 'common/fade/FadeAnimation'
import CommonGallary from 'common/gallary/Gallary'
export default{
	name: 'DetailBanner',
	data () {
		return {
			showGallary: false,
			imgs: ['http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_800x800_70debc93.jpg','http://img1.qunarzz.com/sight/p0/1709/76/7691528bc7d7ad3ca3.img.png_800x800_9ef05ee7.png']
		}
	},
	methods: {
		handleBannerClick () {
			this.showGallary = true
		},
		hanleGallaryClose () {
			this.showGallary = false
		}
	},
	components: {
		CommonGallary,
    FadeAnimation
	}
}
</script>

<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color:#fff
      background-image: linear-gradient(top,rgba(0,0,0,0),rgba(0,0,0,8))
      .banner-tittle
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        line-height: .32rem
        height: .32rem
        margin-top: .14rem
        padding: 0 .4rem
        border-radius: .2rem
        background: rgba(0,0,0,.8)
        font-size: .32rem
        .banner-icon
          font-size: .32rem
</style>