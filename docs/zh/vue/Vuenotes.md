
```
v-for  遍历
v-if v-else v-else-if  控制元素是否插入
v-show  控制元素显示隐藏
v-html  跟{{}}一样，控制元素的innerHTML
v-text
v-bind   简写为 ：  绑定标签的属性
v-on  简写为@ 给标签绑定事件
v-module 实现双向绑定，主要针对表单元素


vue生命周期：
beforeCreate  //初始化 配置项未挂载在实例（处理 data,props,propsData,computed,method,watch）
created      //初始化完成，配置项分配到实例
beforeMount  //dom节点未生成前(渲染视图)
mounted     //dom节点加载完成  
beforeUpdate   //数据发生变化，但是dom未完成  （更新）
updated     //dom节点更新完成
beforeDestroy  //
destroyed





setup(app){
    app.get("/api/data",function(req,res){
        res.json({mes:"success"})
    })
}    setup中的代码不会去运行，它相当于node的进程 


method(){
    axios.get("/api/data").then(res=>{
        this.mes=res.data
    })
}






```



```
安装：cnpm install -g vue-cli
      yarn install -g vue-cli
      yarn 包管理器
      cnpm install -g yarn  //
      cnpm install-g cnpm
使用：vue init webpack(目录)
      vue init webpack-simple (目录)   简易版


组件：
    .vue是vue组件的一种实现
    vue-loader
    
    <template>
        <--只有一个根节点元素-->
    </template>
    <script></script>
    <style></style>
    
    vue-template-compiler
    vue-style-loader
    
    
    1.cnpm install --save-dev vue loader
    const{vueLoaderPlugin}=require("vue-loader")
    {
        test:/\.vue$/,
        loader:"vue-loader"
    }
    2.cnpm install --save-dev vue-template-compiler
    3.cnpm install --save-dev vue-loader
    
    vue中data定义属性时，data必须是一个函数返回一个{}
```

