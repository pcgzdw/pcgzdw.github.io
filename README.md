# express 程序建立：
### 一、前提：
 #### 1、安装好node.建立保存应用程序的文件夹并把该文件夹做为当前目录:(mkdir myapp; cd myapp),运行cnpm init建立你的应用程序并创建相应的package.json 文件，安装好 Express作为依赖项，新建一个app.js文件包括如下代码
`const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})`
就完成了一个最简单的express应用程序;
 #### 2、安装好Express 生成器 cnpm install -g express-generator
### 二、文本复制：ctrl+shift+方向键（含home end键）
### 三、删除操作：先选定内容再按delete键,ctrl+shift+k可直接删除当前行
### 四、剪切操作：ctrl+x可直接剪切当前行，alt+上下方向键可将该行直接上下移动或将选中的多行上下移动。
### 五、alt+shift+上下方向键可将当前行复制到当前行的上下，或将选中的多行复制到当前行的上下。
### 六、ctrl+enter可在当前行的下面新开一行，ctrl+shift+enter可在当前行的上面新开一行。
### 七、撤消光标移动ctrl+u可撤消上一次光标的移动。
### 八、alt+上下方向键可把当前行上下移动。

function bar（）
{
    foo();    
}
你好
你好
你好
