Examples
-------------------------

+ 第一步：安装node
- sudo npm install
+ 第二步：安装bower
- npm install bower -g
+ 第三步：安装rsvp依赖包
- bower install
+ 第四步：启动node
- node server.js
+ 第五部：访问页面
+ [滚动显示](http://localhost:8080/app/html/continuous.html) 鼠标滚动连续显示
+ [单页翻页](http://localhost:8080/app/html/spread.html) 利用columns css属性为页面分栏
+ [双页翻页](http://localhost:8080/app/html/spread.html)  用svg制作的一个图片，可以添加删除图片中的树木

---------------------------
+ 项目结构
- epubjs-------------------------------------项目名称
+  app-----------------------------------应用
-    books---------------------------书籍所在文件夹
+      build----------------------------合并压缩后的js文件所在文件夹
-      controllers----------------------可用于添加笔记或者书签的js所在的文件夹
+      css-------------------------------css文件所在的文件夹
-		hooks----------------------------钩子脚本所在的文件夹
+		html------------------------------主页所在的文件夹
-			continuous.html-----------滚动显示
+			spread.html----------------单页显示
-			spreads.html---------------双页显示
+		images---------------------------存放切图的照片
-		js----------------------------------存放js
+			book.js----------------------存放对整本书的操作的方法
-			continuous.js---------------滚动显示的分支
+			core.js-----------------------存储全局方法
-			epub.js----------------------封装接口
+			hooks.js---------------------钩子脚本
-			layout.js---------------------对章节排版
+			map.js-----------------------计算每页的起始节点
-			navigation.js----------------对目录的处理
+			paginate.js-------------------翻页显示的分支
-			parser.js----------------------解析书籍
+			queue.js----------------------队列脚本
-			rendition.js------------------控制页面的显示与加载
+			replacements.js-------------对页面里的链接什么的做处理
-			section.js--------------------每一章的基本信息
+			view.js-----------------------控制view
-			views.js----------------------管理view
+	bower_components-------------------存放bower下载的js库
-	node_modules-------------------------存放node下载的nodejs库
+	.bowerrc--------------------------------管理存放bower下载的js库的文件夹名称
-	.gitignore-------------------------------管理git忽略的文件
+	bower.json------------------------------bower的配置文件
-	Gruntfile.js-----------------------------压缩与加密js
+	package.json---------------------------node的配置文件
-	README.md
+	server.js---------------------------------node.js用于模拟后台

-----------------