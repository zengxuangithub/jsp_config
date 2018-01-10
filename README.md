# jsp_config配置
```


<jsp-config>
  	<jsp-property-group>
  	
  		<!-- 表示对哪些文件进行配置 -->
  		<url-pattern>/test/*</url-pattern>
  	
  		
  		<!-- 忽略表达式  如果设置为true 
  		则会原封不动直接输出表达式内容 -->
  		<el-ignored>true</el-ignored>
  		<!-- 页面编码字符集  
  		相当于<@ page pageEncoding="UTF-8"> 的设置 -->
  		<page-encoding>UTF-8</page-encoding>
  		
  		<!-- 不 允许使用java 脚本吗-->
  		
  		<!-- 如果设置不允许   该页面会跳转tomcat报错页面  
  		显示  jsp:expression  are disallowed here. -->
  		<scripting-invalid>true</scripting-invalid>
  		
  		<!-- 隐式导入页面头  后缀名为.jspf--> 
  		<include-prelude>/inc/top.jspf</include-prelude>
  		
  		
  		<!-- 隐式导入页面底部缀名为.jspf--> 
  		<include-coda>/inc/bottom.jspf</include-coda>
  	</jsp-property-group>
  	
 </jsp-config>

```









---

#  jspf  
jspf可以直接读取xml文件所以可以 引入公共部分如下
-  jsp 的自定义标签 taglib 也可以用  
-   公共css 
-   公共js
-   等页面公用部分
-   <%@ page >

