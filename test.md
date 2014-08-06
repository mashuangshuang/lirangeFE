YII 前端开发
============

使用YII前端需要注意的问题
##YII
Yii是一个`基于组件`、用于开发大型 Web 应用的 高性能 PHP 框架,yii所拥有的特性包括MVC、DAO/ActiveRecord，							caching、`基于 JQuery 的 AJAX 支持`、用户认证和基于角色的访问控制、脚手架、输入验证、`部件`、事件、主题化以及 Web 服务等等。Yii 采用严格的 `OOP 编写`，Yii 使用简单，非常灵活，具有很好的可扩展性;


##页面布局（layout)

根据设计图，确定页面的布局方式，是全屏布局，上左右布局等等

WebRoot/protected/views/layouts: 此目录放置所有布局视图文件					
	WebRoot/protected/views/layouts								
		|- full.php  												
		|- main-left.php 

WebRoot/protected/views/        此目录下存放action视图文件																	
以一个controller为view目录，以一个controller中action渲染相应view下的文件

如：天风官网中信息公告为例																										

controller/Noticep																										
	action: Notice/company 	公司经营公告   	 view/about/comnpay.php															
	action:	notice/employ   从业人员公告   	 view/about/amploy.php 														


##ui组件##																													
1.物件(widgets)																									
2.组件(CComponent)																												
3.模块(module)：包含模型, 视图, 控制器 和其他支持的组件，大型应用可以划分成通用的功能，例如用户管理， 评论管理  																				

常用的物件：menu,listview,CBreadcrumbs  									

常用的组件：可以根据项目的实际情况进行开发；例如：天风官网中联系我们															

常用的模块：form表单，

##主要学习部分																														
权威指南下：模型-视图-控制器 (MVC)，视图，组件，模块，开发规范，开发流程																
类参考手册：zii-widgets,zii-widgets-grid,zii-widgets-jui

##其他注意的问题##
路径问题：脚本路径，图片路径，链接路径都要通过yII输出																			
开发中遇到的问题，看看YII是否提供的相关解决方案，这就需要我们详细查阅api;
