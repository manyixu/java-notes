> *作用JAVA程序员，用了这么多年的TOMCAT，你居然不知道TOCMAT各个目录的作用及内容，you are out?<br/>*
> *注:本文不会讲什么是TOMCAT,TOMCAT的作用及原理等问题<br/>*
> *关于作者:qq375461826*
#*tomcat文件目录不完全指北*
***

+ ### bin
	目录主要是用来存放tomcat的命令、脚本。
   一类是以「.sh」结尾的（linux脚本），一类是以「.bat」结尾的（windows脚本）。
+ ### conf
	目录主要是用来存放tomcat的一些配置文件。	  
	+ server.xml可以设置端口号、设置域名或IP、默认加载的项目、请求编码
	+ web.xml可以设置tomcat支持的文件类型
	+ tomcat-users.xml用来配置管理tomcat的用户与权限
	
+ ### lib
	主要用来存放tomcat运行需要加载的jar包
+ ### logs
	用来存放tomcat在运行过程中产生的日志文件
+ ### temp
	用户存放tomcat在运行过程中产生的临时文件
+ ### webapps
	用来存放应用程序，当tomcat启动时会去加载webapps目录下的应用程序。可以以文件夹、war包、jar包的形式发布应用。当然，你也可以把应用程序放置在磁盘的任意位置，在配置文件中映射好就行。
	+ ROOT 为根网站，也就是访问localhost:8080 时的页面项目,删除后无法访问;通过这个页面可以跳转到许多其它的webapps下项目的页面
	+ examples 一个示例项目
	+ Manager 项目页面可以管理其它发布的项目，如examaples，也可以管理你以后发布的项目，在它的页面上可以对所有的被管理项目进行启动、停止、重启操作。
	+ **在默认情况下，Tomcat Manager是处于禁用状态的**。准确地说，Tomcat Manager需要以用户角色进行登录并授权才能使用相应的功能，不过Tomcat并没有配置任何默认的用户，因此需要我们进行相应的用户配置之后才能使用Tomcat Manager。<br/>
	配置方法:<br/>
		 `<role rolename="manager-gui"/>` <br/>
		 `<role rolename="admin-gui"/>` <br/>
 		 `<user username="admin" password="123456" roles="manager-gui,admin-gui"/>`
	######*ps:话说回来,如果没有默认禁用这个功能的话,那么运行TOMCAT下的项目是多么的不安全*
+ ### work
	work目录用来存放tomcat在运行时的编译后文件，例如JSP编译后的文件。清空work目录，然后重启tomcat，可以达到清除缓存的作用。

> *感谢阅读，后面如果有新的知识点也会添加进去*