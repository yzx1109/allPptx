###flex
	适用场景: PC布局用的少,在移动端大量使用
	HTML5的新特性在PC端的支持不咋的,而在移动端上支持的很好
	PC端在上浏览器的内核不同:
		IE:  				 Trident         
		FireFox:  			 Gecko 
		Chrome,Safari        webkit    
		Opera  				 Presto

	而在移动端上浏览器内核统一,都是基于webkit的内核
	容器
		display: flex; 必须将盒子显示的定义为flex盒子

		flex-direction
			主轴的方向或项目的排列方向
				row    从左到右  默认值
				column  从上到下
				row-reverse  从右到左
				column-reverse 从下到上


		flex-wrap
			项目是否在一行显示
			nowrap    不换行    默认值
			wrap      换行      
			wrap-reverse   	   换行反转 

		flex-flow
			是flex-direction和flex-wrap的复合属性

		justify-content
			项目在主轴上的对齐方式
				flex-start  主轴的起始边对齐
				flex-end    主轴的结束边对齐
				center      主轴居中对齐 
				space-between  两端没有距离
				space-around   两端有距离



		align-items
			项目在交叉轴上的对齐方式
				flex-start  交叉轴的起始边对齐
				flex-end    交叉轴的结束边对齐
				center      交叉轴居中对齐 
				stretch     拉伸
				baseline    基线,有文本的时候用
		align-content
			适用于多行或多列的flex容器在交叉轴上的对齐方式
				flex-start  交叉轴的起始边对齐
				flex-end    交叉轴的结束边对齐
				center      交叉轴居中对齐 
				stretch     拉伸
				space-between  交叉轴两端没有距离
				space-around   交叉轴两端有距离








	项目
		order
			项目的排列顺序   默认值零  order越大越靠后
		flex-grow
			项目的放大比例 
				默认值是零,也就是当容器有剩余空间,项目不会放大

				是1, 项目平分容器的主轴空间

		flex-shrink
				默认值是1,项目等比例缩小

		flex-basis
			   固定空间,相当于width属性
		flex
			flex-gro（0） flex-shrink(1) flex-basis(auto)的三个复合属性
			推荐使用复合属性
			flex: 1;  项目平分容器的主轴空间
		align-self
			可以单独设置每个项目在交叉轴上的对齐方式
			默认继承align-items的值









