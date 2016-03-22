## This is task 2 readme 
css居中总结    
通常我们用到的css布局都是左右居中，经典css写法如下：

				body{  
				    margin:0;  
				    padding:0;  
				    width:100%;  
				    height:100%;  
				}  
				div{  
				    margin:0 auto;  
				    width:500px;  
				    height:auto;  
				}  
上面是经典的左右居中的css写法，那么像登录框那些比较小得div块只是左右居中是否不是太美观，如果上下左右都居中这是
大多数网站的做法，下面是一个比较经典的div上下左右居中的css写法：

				body{  
				    margin:0;  
				    padding:0;  
				    width:100%;  
				    height:100%;  
				}  
				div{  
				   position:absolute;  
				   top:50%;  
				   left:50%;  
				   margin-top:-250px;  
				   margin-left:-250px;  
				    /*此时宽和高都要固定*/  
				    width:500px;  
				    height:500px;  
				}  

上面的margin可以合并：margin:-250px 0 0 -250px;
大概原理就是：布局需用position，绝对布局absolute还是相对布局relative得看父容器，top，left相对于顶部和左部都相距整个容器的50%，然后在利用margin，向上回退div高的50%即：margin-top:-250px
向左回退div宽的50%即：margin-left:-250px 
