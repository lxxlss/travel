<template>
	<div class="header">
	  <div class="header-left">
	  	<span class="iconfont">&#xe6b7;</span>
	  </div>
	  <div class="header-input">
	  	<span class="iconfont">&#xe633;</span>
	  	输入城市/景点/游玩主题
	  </div>
	  <!--点击跳转city页面-->
	  
	  <div class="header-right">
	  	<router-link to='/city'>
	  	{{this.city}}
	  	<span class="iconfont">&#xe600;</span>
	   </router-link>
	  </div>
	  
	</div>
</template>

<script>
	 export default {
	 	name:'HomeHeader',
	 	props: {
	 	   city: String
	 	}
	 }
</script>

<style lang="stylus" scoped>
 @import '~styles/varibles.styl'
/*1rem = html font-size =50px (86/100)*/
  .header
    width:100%
    display:flex
    height:$headerHeight
    line-height:$headerHeight
    background:$bgColor
    color:#fff
    .header-left
       width:8%
       float:left
       color:#fff
    .header-right
       width:17%
       float:right
       text-align:center
    .header-input
       padding-left:0.1rem
       flex:1
       background:#fff
       height:0.6rem
       margin-top:0.1rem
       border-radius:0.1rem
       color:#ccc
       line-height:0.6rem
</style>