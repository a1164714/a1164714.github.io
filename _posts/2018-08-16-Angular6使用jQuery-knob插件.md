---
layout:     post
title:      Angular6使用jQuery-knob插件
subtitle:   Angular4升级Angular6后，引入JS插件变得异常简单
date:       2018-08-16
author:     Littleevil
header-img: img/post-bg-angular6-jqueryKnob.jpg
catalog: true
tags:
    - Angular
    - 前端
    - jQuery-knob
---
### 1、概述

Angular想使用jQuery-knob和jQuery是一样的操作。

> Angular6引入jQuery变得异常简单，请参考https://blog.csdn.net/qq_35321405/article/details/80270496
>

### 2、简单流程

- yarn add jquery 或者 npm install jquery --save（后面省略或的内容）
- yarn add @types/jquery
- yarn add jquery-knob
- yarn add @types/jquery-knob

```
// componnet的头部引入
import * as $ from 'jquery';
import 'jquery-knob';

// componnet中使用
ngOnInit(): void {
    $(function() {
      $(".dial").knob();
    });
}

// html中
<input type="text" value="75" class="dial">
```

> 代码参考：https://github.com/a1164714/jquery-knob-demo