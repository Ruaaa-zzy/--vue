<template>
  <div id="app">
	        <!-- <router-link to="/">Home</router-link> | -->
      <!-- <router-link to="/about">About</router-link> -->
    <!-- <div id="nav">

    </div> -->
	<!-- 顶部导航 -->
	<NavTop  />
	<!-- 渲染内容 -->
    <router-view/>
  </div>
</template>

<script>
import NavTop from '@/components/nav_top.vue';
export default {
	data() {
		return {
			
		}
	},
	components: {
		NavTop
	}
}
</script>
<style lang="scss">
@import '@/assets/css/comment.scss'

</style>
