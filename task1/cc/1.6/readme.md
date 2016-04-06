# task 6
## [三栏布局我知道的有三种方法](https://github.com/hawx1993/Front-end-Interview-questions#css实现三栏布局中间自适应）
1. CSS透明度设置（兼容所有浏览器）
				.transparent_class {  
		     	 	filter:alpha(opacity=50);  
		      		-moz-opacity:0.5;  
		      		-khtml-opacity: 0.5;  
		      		opacity: 0.5;  
					} 

2. css font-variant语法
	font-variant : normal | small-caps
	normal : 正常的字体
	small-caps : 让字母变成小型的大写字母字体并缩小字母
	
3. 绝对定位法。左右两栏采用绝对定位，分别固定于页面的两侧，中间的主题栏用左右margin撑开距离。    
无顺序要求。