说明：

   原生JavaScript常用交互方法大杂烩

场景/需求：
   
   运用以下各知识点新窗口访问目标网址，如“https://github.com/”。



知识点梳理：

1. // 输出内容：直接向HTML输出流写内容，即直接在网页中输出内容。

   document.write();


2. // alert 警告（包含一个确定按钮）【调试】
   
   alert(字符串或变量);


3. // confirm 确认（包含一个确定按钮和一个取消按钮）【允许用户做选择】
   
   confirm(str);

   ·str：在消息对话框中要显示的文本

   ·返回值：Boolean值【确定 - true | 取消 - false】- 通过返回值可以判断用户点击了什么按钮


4. // prompt 提问（包含一个确定按钮，取消按钮与一个文本输入框）【用于询问一些需要与用户交互的信息】

   prompt(str1, str2);

   ·str1：要显示在消息对话框中的文本，不可修改
   
   ·str2：文本框中的内容，可修改

   ·返回值【确定 - 文本框中的内容将作为函数返回值 | 取消 - 返回null】


5. // 打开窗口
 
   window.open([url], [窗口名称], [参数字符串]);

   ·open() 方法可以查找一个已经存在或者新建的浏览器窗口。
   
   ·url：可选参数，在窗口中要显示网页的网址或路径。如果省略这个参数，或者它的值是空字符串，那么窗口就不显示任何文档。

   ·窗口名称：可选参数，被打开窗口的名称。
    	
	1. 该名称由字母、数字和下划线字符组成；
	
	2.“_top”“_blank”“_self”具有特殊意义：
	
	   ·_top：在上部窗口中显示目标网页。

	   ·_blank：在新窗口显示目标网页。

	   ·_self：在当前窗口显示目标网页。

	3. 相同name的窗口只能创建一个，要想创建多个窗口则name不能相同。

   ·参数字符串：可选参数，设置窗口参数，各参数用逗号隔开【参数表见图 - args.png】


6. // 关闭窗口

   window.close();【关闭本窗口】
   
   <窗口对象>.close();【关闭指定窗口】


   
学习心得：

   死记硬背单纯的知识点是枯燥乏味且不可取的，理应结合具体场景活学活用。






