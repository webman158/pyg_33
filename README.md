## 初始wepy

# 1. 全局安装或更新WePY命令行工具
```bash
npm i wepy-cli -g
```

# 2. 初始化项目
```bash
wepy init standard my-project

standard ==>  promise  async
empty   空的模板
```

# 3. 切换至项目目录
# 4. 安装依赖
```bash
cd my-project

npm i
```

```bash
开启实时编译
wepy build --watch  ==> npm run dev
```

使用微信开发者工具用来查看效果和调试
写代码使用vscode


## 每个文件的作用
1. dist  ==> 打包后的小程序的代码
2. src   ==> 开发目录


## 让vscode 支持对wpy文件的高亮效果
1. 安装vuter 插件
2. 任意打开一个wpy文件， 选择右下角的纯文本
3. 选择.wpy 文件的配置关联
4. 选择vue


或者是直接把下面代码加入到设置中
```json
"files.associations": {
      "*.wpy": "vue"
  }
```

## wpy 文件
style ==> 写样式 ，支持less    wxss文件
template  ==>   写结构的      wxml文件
script（除了config部分） ==> 对应的js文件   js文件
script(config部分)    ==>  对应的json文件   json文件


在wepy框架中，小程序页面的四个组成部分，现在都在一个wpy文件中


## 使用git 管理项目
1. git init
2. git status
3. git add .
4. git commit -m "提交信息"
5. git remote add origin git@github.com:webman158/pyg_33.git
6. git push -u origin master


## 配置pages + window
注意： 在app.wpy文件中 config 部分中配置的
