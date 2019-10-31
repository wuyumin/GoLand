# 常用配置

> - File -> Default Settings 默认设置。
> - File -> Settings 当前项目设置。注意：有些默认设置也通过此设置来实现。
> - 所有设置完毕后都要 Apply（应用）或 OK（确认）后才能生效。

### 取消自动保存并标识修改的文件为星星标记

- 取消自动保存：File -> Settings -> Appearance & Behavior ->System Settings 去掉勾选Save files on frame deactivation
- 使用星星标记：File -> Settings -> Editor -> General -> Editor Tabs 勾选Mark modifyied tabs with asterisk

### 如何显示行号？

如果你的编辑区没有显示行号，可以通过以下设置来进行显示 File -> Settings -> Editor -> General -> Appearance 标签项，勾选 Show line numbers。

### 启动时不打开项目？

File -> Settings -> Appearance & Behavior ->System Settings 去掉勾选Reopen last project on startup

### 常用文件模板设置

File -> Settings -> Editor -> File and Code Templates

### 单行注释符号后加空格？

File -> Settings -> Editor -> Code Style -> Go -> Other 标签项，去掉勾选 Line comment at first column 而勾选 Add a space at comment start。

### 取消方法(函数)的参数值前面的文字提示？

File -> Settings -> Editor -> General -> Appearance 去掉勾选 Show parameter name hints。

### jQuery 代码提示？

File -> Settings -> Languages & Frameworks -> JavaScript -> Libraries
1. 自动安装(推荐)：右边 Download... -> TypeScript community stubs 选择 jquery 来自动下载安装。
2. 手动安装：右边 Add... （后面步骤跟自动安装后的填写差不多，可以先自动安装后再自定义自己的）。
提示：说明文档 Documentation URLs 那里的 http://api.jquery.com 可以下载到本地以加快显示速度。

### 如何添加插件？

File -> Settings -> Plugins -> Browse repositories -> 搜索  
常用的代码提示插件有：Bootstrap、AngularJS(有些版本已自动带了)、Vue.js 等等

### 如何去掉右上角浏览器图标？

File -> Settings -> Tools -> Web Browsers 下面去掉勾选 Show Browsers popup in the editor

### 默认展开头部注释

File -> Settings -> Editor -> Genaral -> Code Folding 去掉勾选 File header

### 默认展开 import 语句

File -> Settings -> Editor -> Genaral -> Code Folding 去掉勾选 Imports

### 一些语言及其版本设置

默认设置 File -> Settings -> Languages & Frameworks 各个语言选项

### 是否保存相关密码

配置搜 password 项

### 是否显示代码里的空格

配置搜 Show whitespaces 项

### 取消在文字里按 Enter 键后自动缩进

File -> Settings -> Editor -> Genaral -> Smart Keys -> Enter 去掉勾选 Smart indent

### Go语言编辑器设置

File -> Settings -> Editor -> Code Style -> Go。

### Node.js设置

File -> Settings -> Languages & Frameworks -> Node.js and NPM 设置一下 Node.js 和 NPM 包的所在位置，并启动助手来增加语法提示功能。如Node.js位置`D:\nodejs\node.exe` NPM 包位置`D:\nodejs\node_modules\npm`。

### 快捷键设置

File -> Settings -> Keymap

### 保存代码时自动格式化代码

`建议设置 Level 全部设置为 Global ，方便所有项目都能使用`

[Go语言]  
保存代码时，自动调用 gofmt 和 goimports 来格式化代码。  

菜单 File -> Settings -> Tools -> File Watchers 分别添加`gofmt`和`goimports`模板。  
gofmt作用：格式化代码  
goimports作用：格式化导入的包  

[Node语言]  
代码格式化
全局安装prettier `npm i prettier -g` (环境变量路径中能直接调用命令)  
安装Prettier插件  
菜单 File -> Settings -> Tools -> File Watchers 添加`Prettier`模板，Program填写全局能使用的`prettier`命令。  
  
prettier配置(使用单引号等)  
项目根目录下`.prettierrc`
```json
{
  "singleQuote": true,
  "printWidth": 120,
  "tabWidth": 2,
  "bracketSpacing": false
}
```

代码语法检查
全局安装eslint `npm i eslint -g` (环境变量路径中能直接调用命令)  
安装ESLint插件  