<template>
	<div class="header">	
	  城市选择
	  <!--回到首页-->
	<router-link to="/">
	 <span class="iconfont header-back">&#xe6b7;</span>
	</router-link></div>
</template>

<script>
	 export default {
	 	name:'CityHeader'
	 }
</script>

<style lang="stylus" scoped>
 @import '~styles/varibles.styl'
/*1rem = html font-size =50px (86/100)*/
  .header
   position:relative
   overflow:hidden
   height:$headerHeight
   line-height:$headerHeight
   text-align:center
   color:#fff
   background:$bgColor
   font-size:.32rem
   .header-back
     width:.64rem
     text-align:center
     font-size:.4rem
     position:absolute
     top:0
     left:0
</style>