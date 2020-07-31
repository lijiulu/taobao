<!-- 主页home right组件  -->
<template>
<div class='app-home-right'>
    <div class="home-right-search ">
        <input type="text" >
        <button>搜索</button>
    </div>
    <div class="warp-home-right-login">
        <div class="home-right-login">
            <div class="right-login-hint">登录可以保存你的浏览爱好、评论、收藏，并与APP同步，更可以发布微头条</div>
            <button>登录</button>
            <div class="right-login-select">
                <span>🐧</span>
                <span>🗨</span>
            </div>
        </div>
    </div>
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';

export default {
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {

};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合
methods: {

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
}
</script>
<style lang='less' scoped>
.app-home-right {
    margin-left: 20px;
    padding: 5px;
  .home-right-search{
      height: 40px; 
      display: flex;
    input {
        flex: 8;
        height: 36px;
        border:1px solid rgb(32,142,218);
        outline: none;
        float: left;
        border-right: none;
        border-radius: 5px 0px 0px 5px;
        font-size: 20px;
        padding-left: 10px;
    }
    button {
        flex: 2;
        height: 40px;
        border:1px solid rgb(32,142,218);
        float: left;
        background: rgb(32,142,218);
        border-radius: 0px 5px 5px 0;
        color: #fff;
        cursor: pointer;
    }
  }

  .warp-home-right-login {
      background: rgba(238, 236, 236, 0.867);
      padding: 15px;
      margin-top:15px ;
    .home-right-login { 
        background-color: rgb(255,255,255);
        padding: 20px;
      .right-login-hint {
          font-size: 12px;
          color: rgb(138, 137, 137);
     }

      button {
          width: 100%;
          height: 40px;
          border-radius: 5px;
          border: none;
          background: rgb(237,64,64);
          margin-top: 20px;
          margin-bottom: 15px;
          color: #fff;
          cursor: pointer;
          outline: none;
      }
      button:hover{
          background-color: rgba(239,83,83);
      }

      .right-login-select {
         
        span {
            display: inline-block;
            width: 40px;
            height: 40px;
            border: 1px solid #000;
            border-radius: 50%;
            text-align: center;
            line-height: 40px;
            margin-left:10px ;
            cursor: pointer;
        }
      }
    }
  }
}
</style>