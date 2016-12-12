# escapeSvg 介绍

将 svg 转换成 URL 编码的 sass 函数。作用是在sass中使用内联 svg。

# escapeSvg 的用法

语法如下
```scss
escapeSvg($string);
```

具体实例如下：
```
$svg: '<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="xMidYMid" viewBox="0 0 750 400">
			<path d="M0,0 L750,0 L750,400 L388,400 L375,387, L362,400 L0,400Z" fill="#0f0"></path>
		</svg>';
background: url(#{escapeSvg($svg)}) 0 0 no-repeat;
background-size: 100% 100%;
```
