# 常用配置

### 保存代码时自动格式化代码

保存代码时，自动调用 gofmt 和 goimports 来格式化代码。  

菜单 File -> Settings -> Tools -> File Watchers 分别添加`gofmt`和`goimports`模板。  
gofmt作用：格式化代码  
goimports作用：格式化导入的包  

`建议以上设置项 Level 全部设置为 Global ，方便所有项目都能使用`
