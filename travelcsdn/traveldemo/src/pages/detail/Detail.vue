<template>
	<div class="detail">
    <detail-banner></detail-banner>
	</div>
</template>

<script>
import DetailBanner from './components/Banner'
export default {
        name:'Detail',
        components:{
          DetailBanner: DetailBanner
         }
	 }
</script>

<style lang="stylus" scoped>
 @import '~styles/varibles.styl'
/*1rem = html font-size =50px (86/100)*/
  
</style>