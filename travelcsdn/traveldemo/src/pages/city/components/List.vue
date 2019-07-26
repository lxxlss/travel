
<template>
 <div class="list wrapper" ref="wrapper">
 	<div>
  <div class="area">
  <div class="title border-topbottom">当前城市</div>
  <div class="button-list">
   <div class="button-wrapper">
   	<div class="button">北京</div>
  </div>
  </div>
  </div>
  <div class="area">
  <div class="title  border-topbottom">热门城市</div>
   <div class="button-list">
	<div class="button-wrapper">
    	<div class="button">北京</div>
    </div>
      <div class="button-wrapper">
   	<div class="button">北京</div>
   </div>
      <div class="button-wrapper">
   	<div class="button">北京</div>
   </div>
      <div class="button-wrapper">
   	<div class="button">北京</div>
   </div>
    <div class="button-wrapper">
   	<div class="button">北京</div>
   </div>
  </div>
  </div>
  <div class="area">
  <div class="title  border-topbottom">A</div>
  <div class="item-list">
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  </div>
  </div>
   <div class="area">
  <div class="title  border-topbottom">A</div>
  <div class="item-list">
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  </div>
  </div>
   <div class="area">
  <div class="title  border-topbottom">A</div>
  <div class="item-list">
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  	<div class="item border-bottom">阿拉尔</div>
  </div>
  </div>
  </div>
 </div>



</template>

<script>
  import Bscroll from 'better-scroll'
  export default {
	 	name:'CityList',
	 	 mounted() {
         this.$nextTick(() => {
	        this.scroll = new Bscroll(this.$refs.wrapper, {})
	      })
	    }
	 }
</script>
<style lang="stylus" scoped>
 @import '~styles/varibles.styl'
	.border-topbottom
	   &:before
	     border-color:#ccc
	   &:after
	     border-color:#ccc
	.border-bottom
	   &:before
	     border-color:#ccc
	   &:after
	     border-color:#ccc
	.list
	 overflow:hidden
	 position:absolute
	 top:1.68rem
	 left:0
	 right:0
	 bottom:0
	 .title
	  line-height:.5rem
	  background:#eee
	  padding-left:.2rem
	  color:#666
	 .button-list
	  padding:.1rem .6rem .1rem  .1rem 
	  overflow:hidden
	  .button-wrapper
	   float:left
	   width:33.33%
	   .button
	    text-align:center
	    margin:.1rem
	    padding:0.1rem 0
	    border-radius:.06rem
	    border:.02rem #ccc solid
	 .item-list
	  .item
	   line-height:.70rem
	   padding-left:.2rem
   
</style>



