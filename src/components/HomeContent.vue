<!-- 中间内容 -->
<template>
<div class='app-home-content'>
    <div class="home-content-haeder">
        <div class="content-haeder-bar"
            v-for='item,index in bar'
            >{{item.text}}</div>
    </div>
    <div class="content-textarea">
        <textarea placeholder="有什么新鲜的事想告诉大家"> </textarea>
    </div>
    <div class="content-floot">
        <div class="content-floot-left">
            <div>
                <img src="http://sf1-ttcdn-tos.pstatp.com/obj/ttfe/toutiao.com/image-icon.png" alt="">
                图片
            </div>
            <div>🙂表情</div>
        </div>
        <div class="content-floot-right">发布</div>
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
    bar:[
        {id:1,text:'发微头条'},
        {id:1,text:'写文章'},
        {id:1,text:'提问题'},
        {id:1,text:'发视频'}
    ]
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
.app-home-content {
    border: 1px solid #dddddd;
  .home-content-haeder {
      height: 40px;
      line-height: 40px;
      font-size: 15px;
    .content-haeder-bar {
        float: left;
        margin-right: 20px;
        text-align: center;
        cursor: pointer;
    }
  }
  .content-textarea {
        height: 100%;
    textarea {
        box-sizing: border-box;
        width: 100%;
        height: 100px;
        padding: 5px;
        font-weight: 200;
        resize: none;
        border: none;
        background: #f4f5f6;
        display: block;
    }
  }

  .content-floot {
      height: 40px;
      display: flex;
      justify-content: space-between;
    .content-floot-left {
       line-height: 40px;
       display:flex;
      
      div {
          display:flex;
          margin-left: 10px;
          align-items: center;
          cursor: pointer;
          img{
              height: 25px;
             
          }
      }
    }

    .content-floot-right {
        width: 100px;
        height: 40px;
        line-height: 40px;
        text-align: center;
        background: rgba(244,140,140);
        color: #fff;
        cursor: pointer;
    }
  }
}
</style>