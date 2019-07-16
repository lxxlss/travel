<template>
	<div class="header">
	  <div class="header-left">返回</div>
	  <div class="header-input">内容</div>
	  <div class="header-right">城市</div>
	</div>
</template>

<script>
	 export default {
	 	name:'HomeHeader'
	 }
</script>

<style lang="stylus" scoped>
/*1rem = html font-size =50px (86/100)*/
  .header
    width:100%
    display:flex
    height:1rem
    line-height:1rem
    background:#00bcd4
    color:#fff
    .header-left
       width:10%
       float:left
    .header-right
       width:15%
       float:right
       text-align:center
    .header-input
       flex:1
       background:#fff
       height:0.5rem
       margin-top:0.5rem
       border-radius:0.2rem
       color:#ccc
       line-height:0.5rem
</style>