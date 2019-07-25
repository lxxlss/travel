<template>
	<div>
	<swiper :options="swiperOption"  ref="mySwiper" @someSwiperEvent="callback">
    <!-- slides -->
    <swiper-slide>
    	<img  class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1802/e3/62ce7362ca051d02.jpg_640x200_6db551b7.jpg"/>
    </swiper-slide>
    <swiper-slide>
    	<img  class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1801/93/ce59d182aca07102.jpg_640x200_ba03d44c.jpg"	/>
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
    <div class="swiper-scrollbar"   slot="scrollbar"></div>
  </swiper>
	</div>
</template>

<script>
	export default{
		name:'SwiperTest'
	}
</script>

<style lang="stylus" scoped>
    
	  .swiper-img
	    width:100%
</style>