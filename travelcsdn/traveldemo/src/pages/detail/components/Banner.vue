<template>
	<div>
	<div class="banner" @click="handleBannerClick">
	<img  class="banner-img" src="https://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20197/cef54e99a8e4eae8f089f54adbc7fe3d.jpg">
	<div class="banner-info">
		<div class="banner-title">大连圣亚海洋世界(AAAA景区)</div>
		<div><span class="iconfont banner-icon"></span>39</div>
	</div>
	</div>
	  <common-gallary 
     :imgs="imgs" 
     v-show="showGallary"
     @close="handleGallaryClose"></common-gallary>
	</div>
</template>

<script>
import CommonGallary from 'common/gallary/Gallary'
	 export default {
	 	name:'DetailBanner',
	 	data(){
	 	 return {
	      	showGallary: false,
			imgs: ['http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_800x800_70debc93.jpg','http://img1.qunarzz.com/sight/p0/1709/76/7691528bc7d7ad3ca3.img.png_800x800_9ef05ee7.png']
		}
	 	},
	 	methods:{
	 	handleBannerClick(){
	 	this.showGallary = true
	 	},
	 	handleGallaryClose () {
	 	this.showGallary =false	
	 	}
	 	},
	   components: {
       CommonGallary
	 	}
	 }
</script>

<style lang="stylus" scoped>
 @import '~styles/varibles.styl'
/*1rem = html font-size =50px (86/100)*/
  .banner
   position:relative
   overflow: hidden
   height:0
   padding-bottom:55%
   .banner-img
    width:100%
   .banner-info
    display:flex
    position:absolute
    left:0
    right:0
    bottom:0
    line-height:.6rem
    background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, .8)) //从底部渐变
    color:#fff
    .banner-title
     flex:1
     font-size:.32rem
    .banner-number
     margin-top:.14rem
     padding:0 .4rem
     line-height:.32rem
     height:.4rem
     font-size:.24rem
     border-radius:.2rem
     background:rgba(0,0,0,.8)
</style>