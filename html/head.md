

# Head

head是网页的头。

header是body的头，是h5才有的。



## meta标签

+ 位于文档的头部，不包含任何内容。其属性定义了与文档相关联的名称/值对。

+ 永远位于 head 元素内部。

+ name-content 算是一种协议，被识别的目标发现后，可特殊处理。比如苹果手机定义了一个tag就可以展示对应网页所属的app

  ```
  <meta name="apple-itunes-app" content="app-id=myAppStoreID, affiliate-data=myAffiliateData, app-argument=myURL">
  ```

+ 动态插入meta

  ```
  var oMeta = document.createElement('meta');
  oMeta.name = "apple-itunes-app";
  oMeta.content = "app-id=xxxxxx, affiliate-data=myAffiliateData, app-argument=" + methd('parm');
  // 插入meta标签
  document.getElementsByTagName('head')[0].appendChild(oMeta);
  
  document.getElementsByTagName('head')获取的时整个界面的header的集合，第一个header的下标是0
  ```

+ 重定向

  ```
  <meta http-equiv="refresh" content="10;url=http://www.baidu.com"> // 10s之后刷新，然后跳转到对应网站
  ```

+ 规定字符集

  ```
  <meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
  ```

+ 文档描述

  ```
  <meta name="author"content="w3school.com.cn">
  <meta name="revised"content="David Yang,8/1/07">
  <meta name="generator"content="Dreamweaver 8.0en">
  ```

## Link标签





## base 标签

+ 定义网页的baseUrl，然后其他url就可以用相对路径

+ href：baseUrl

+ target

  ```
  _blank	在新窗口中打开被链接文档。
  _self	默认。在相同的框架中打开被链接文档。
  _parent	在父框架集中打开被链接文档。
  _top	在整个窗口中打开被链接文档。
  framename	在指定的框架中打开被链接文档。
  ```



## script 标签

+ 插入脚本

  ```
  <script type="text/javascript">
  document.write("<h1>Hello World!</h1>")
  </script> 
  ```

+ 浏览器不支持脚本

  ```
  <noscript>Sorry, your browser does not support JavaScript!</noscript>
  ```

+ 属性

  ```
  async	设置或返回是否脚本一旦可用，就应异步执行。
  charset	设置或返回脚本的 charset 属性值。
  cross Origin	设置或返回脚本的 CORS 设置。
  defer	设置或返回当页面完成解析后是否执行脚本。
  src	设置或返回脚本的 src 属性值。
  text	设置或返回属于脚本子节点的所有文本节点的内容。
  type	设置或返回脚本的 type 属性值。
  ```



## style 标签





## title 标签

