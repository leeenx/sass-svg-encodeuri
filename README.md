# sass-svg-encodeuri 介绍

将 svg 转换成 URL 编码的 sass 函数。作用是在sass中使用内联 svg。

# sass-svg-encodeuri 的用法

语法如下
```scss
sass-svg-encodeuri($string);
```

具体实例如下：
```
$svg: '<svg viewBox="0 0 750 400" width="750" height="400">
			<path d="M0,0 L750,0 L750,400 L388,400 L375,387, L362,400 L0,400Z" fill="#0f0"></path>
		</svg>';
background: url(#{sass-svg-encodeuri($svg)}) 0 0 no-repeat;
background-size: 100% 100%;
```
