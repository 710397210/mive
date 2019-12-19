<template>
    <!--template-->
    <div>
        <h1>{{content}}</h1>
        请输入内容：<input type="text" v-model="content">
        <el-button type="warning" round="">按钮</el-button>
    </div>
</template>
<!--template代表的就是html的内容，相当于<div id="app">标签中的内容-->
<script>
    import ElButton from "../../node_modules/element-ui/packages/button/src/button";
    /*<script>*/


    export default {
        //在.vue文件中定义
        components: {ElButton},
        data:function () {
            //return返回数据，将对象通过return返回给vue-cli
            return {
                content:""
        }
        }
    }
</script>
<style scoped>/*scoped含义：将当前vue文件中css属性的作用域限制在当前的页面，不会对其他页面产生影响*/
    h1{
        color: red
    }
</style>