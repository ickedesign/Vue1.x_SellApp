Vue2.x_SellApp
===========================
> 仿饿了吗外卖APP单页[vue, vue-router, vue-resource]

### 环境依赖
node v4.0.0+
npm v3.0.0+

### 部署步骤
1. npm install -g vue-cli
2. vue init webpack sell
3. npm install  
4. npm run dev  

### 项目打包
1. npm run build

### 目录结构描述
```
├── build                  // webpack的基本配置、开发环境配置、生产环境配置等
├── config                 // 路径端口值        
├── src                    // 组件和入口文件                 
│   ├── common             // 存放共有文件
│   |   ├── fonts             
│   |   ├── js         
│   |   └── stylus         
│   ├── components         // 存放组件
│   |   ├── cartcontrol    // 增减商品
│   |   ├── goods          // 商品列表
|   |   ├── header         // 页面头部
|   |   ├── ratings        // 评论列表
|   |   ├── seller         // 商家页面
|   |   ├── shopcart       // 购物车
|   |   └── star           // 星级打分
|   ├── App.vue            // 主组件
|   └── main.js            // 入口文件
├── node_modules           // 依赖的模块
├── static                 // 静态文件
│   └── css
├── .babelrc               // 设置转码的规则和插件
├── .editorconfig          // 设置编辑器
├── .eslintignore          // 设置eslint忽略检查的文件
├── .eslintrc.js           // eslint配置
├── .gitignore             // git提交配置
├── .postcssrc.js          
├── README.md
├── data.json              // Mock数据
├── index.html             // 文件入口
├── package.json           // 定义项目所需模块和配置信息
└── prod.server.js         // 调试文件
```

### 功能和技术
1. 使用vue-cli脚手架完成项目搭建，vue-router做路由，vue-resource实现数据交互
2. 图片根据像素比的不同显示，有DPR为2和DPR为3两种图片
3. 项目使用css的预处理器stylus进行样式编写，使用到了Flex布局,sticky foot布局,还有兼容其它移动端的1像素边框制作
4. 使用mock数据，独立于后端进行开发
5. 使用Eslint来规范代码编写
6. 使用better-scroll插件做页面滚动

### 项目页面
![pageshot](https://github.com/ickedesign/Vue2.x_SellApp/blob/master/pageshot.jpg)
