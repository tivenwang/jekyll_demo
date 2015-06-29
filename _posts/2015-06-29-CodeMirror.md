
---
layout: post
title: CodeMirror-SQLHint使用
---

简单描述下使用场景，应用需要提供一个简单的SQL查询窗口，能够高亮显示SQL语法即可。
##### 1. 获取代码配置依赖
   到codemirror官网上下载下来一套代码，将lib下的```codemirror.js、codemirror.css```文件和mode/sql文件夹下的```sql.js```文件导入到页面中。lib是codemirror的lib，mode是当前使用的语言模式，即SQL语言。
##### 2. 如何使用
   下面的代码展示了如何初始化一个codemirror，以及其的参数配置释义。
 ```
<!-- Create a simple CodeMirror instance -->
<link rel="stylesheet" href="lib/codemirror.css">
<script src="lib/codemirror.js"></script>
<script src="mode/sql/sql.js"></script>
<script>
  var editor = CodeMirror.fromTextArea(myTextarea, {
    lineNumbers: true,//设置行号 boolean
    value: 'SELECT * FROM table',//编辑框初始值 string    
    mode: 'text/x-mysql',//当前code模式 模式的选择可以在CodeMirror.modes中查看

  });
</script>
```