<template>
  <div class="c-nav_top">
    <div class="c-nav_top-content content">
      <div class="c-nav_top-content-left">
        <img src="../static/position.jpg" alt="">
        <p>辽宁</p>
      </div>
      <div class="c-nav_top-content-right flex-between">
        <p class="c-nav_top-content-right-title" @click="aa">你好，请登录<span>&nbsp;&nbsp;免费注册</span></p>
        <p class="c-nav_top-content-right-item" v-for="navValue in nav" :key="navValue">{{ navValue }}</p>
      </div>
    </div>

  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'nav_top',
  data() {
      return {
        nav: ['我的订单','我的京东','京东会员','企业采购','客户服务','网站导航','手机京东']
      }
  },
  methods: {
    aa() {
       this.$router.push({ path:'/a.html'  }) 
    }
  },
  components: {
  }
}
</script>

<style>
.c-nav_top{
  background: #e3e4e5;
  padding: 10px 0;
}
.c-nav_top-content{
  display: flex;
  align-content: center;
}
.c-nav_top-content-left{
  display: flex;
  align-items: center;
  padding-right: 422px;
}
.c-nav_top-content-left img{
  width: 10px;
  height:20px;
  margin-right: 10px;
}
.c-nav_top-content-right-title{
  padding-right:10px;
}
.c-nav_top-content-right-title>span {
  color: #e33333;
}
.c-nav_top-content-right-item{
  padding:0 18px;
  border-left: #000 solid 1px;
}
.c-nav_top-content-right-item,.c-nav_top-content-right-title,.c-nav_top-content-left p{
  font-size: 12px;
}
</style>
