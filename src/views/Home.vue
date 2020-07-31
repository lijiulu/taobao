<template>
  <div class="home">
    <!-- 主页haeder的开始 -->
    <div class="tt-home-header">头条</div>
     <!-- 主页haeder的结束-->
     <!-- 主页中间内容的开始 -->
     <div class="tt-home-content">
       <div class="home-content-left">
         <Navigator></Navigator>
       </div>
       <div class="home-content-middle">
         <HomeContent></HomeContent>
       </div>
       <div class="home-content-right">
         <HomeRight></HomeRight>
       </div>
     </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
//引入left 组件
import Navigator from '../components/Navigator'
//引入 content 组件
import HomeContent from '../components/HomeContent'
//引入right 组件
import HomeRight from '../components/HomeRight'
export default {
  name: 'Home',
  components: {
    HelloWorld,
    Navigator,
    HomeContent,
    HomeRight
  }
}
</script>
<style lang="less">
.tt-home-header{
  height: 50px;
  font-size: 20px;
  font-weight: 200;
  color: #fff;
  padding-left:10px ;
  background: #000;
  line-height: 50px;
  margin-bottom: 10px;
}
.tt-home-content {
  width: 80%;
  min-height: 400px;
  margin: 0 auto;
  display: flex;
  text-align: center;
  .home-content-left {
    flex: 1;
  }

  .home-content-middle {
    flex: 3;
  }

  .home-content-right {
    flex: 2;
  }
}
</style>