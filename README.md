## 一、express 程序建立
 ### （一）前提条件：首先安装好安装好node。
  #### 1、最简单的express程序建立：
   ######  1）建立保存应用程序的文件夹并把该文件夹做为当前目录:(mkdir myapp; cd myapp);
   ######  2）运行cnpm init建立你的应用程序并创建相应的package.json 文件;
   ######  3) 安装好 Express作为依赖项(cnpm install express)，
   ######  4)新建一个app.js文件包括如下代码:

```
const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})
```
   ###### 5) 这就完成了一个最简单的express应用程序;然后在命令行上运行node app.js，并在浏览器中加载 http://localhost:3000/ 以查看输出

  #### 2、使用应用程序生成器工具 express-generator 快速创建应用程序骨架。
   ##### 1）安装好Express 生成器express-generator(cnpm install -g express-generator);
   ##### 2）创建一个名为 myapp 的 Express 应用程序。该应用程序将在当前工作目录中名为 myapp 的文件夹中创建，并且视图引擎将设置为(Pug：express --view=pug myapp)
   ##### 3) 安装依赖(cd myapp;cnpm install)
   ##### 4) 在 Windows 命令提示符上，使用以下命令 set DEBUG=myapp:* & npm start启动服务器程序。
   ##### 5）然后在浏览器中加载 http://localhost:3000/ 以访问该应用程序。

