# servlet

HttpServlet()

​	service

* `doGet()`
* `doPost()`

> `processRequest()`

#### response

> 接口

提供了一个`response.getWriter()`方法，返回PrintWriter对象

~~~java
out=response.getWriter();//返回网页
response.setContentType("text/html,charset='utf-8'");//说明返回的是网页
~~~



#### response接口响应http请求步骤

1. 创建一个servlet类

2. 重写`doGet()`或`doPost()`实现响应

   > 由`service()`方法调用

HttpServletResponse主要从Servlet继承了

1. getWrite
2.   

javaee5规范后，推荐使用注解代替配置文件

* @WebServlet(name="First",urlPattern={"/First"})

* 需要导入javax.servlet.annotation.WebServlet包

  ~~~java
  import javax.servlet.annotation.WebServlet;
  ~~~

* 同时使用注解和配置文件以哪个为准？

  > 注解

Request接口——客户输入参数处理

* Post方法——数据由标准的输入设备读入
* Get方法——数据由CGI Inerface（是HTTP服务器与客户机上的程序进行联系的一种工具变量）QUERY_STRING传递给表单数据……

> 处理方法一致

HttpServletResponse处理方法

1. getParameter()单值
2. getParameterValues()多值
3. getParameterNames()枚举返回参数名列表



`request.getParameter(" ")`使用服务器当前字符集解释输入

改变默认使用`request.setCharaterEncoding("utf-8")`

关于字符集和字符编码

* ASCII码

* GBK

* Unicode

* UTF-8（Unicode TransformationFormat-8bit）

  > 类似哈夫曼编码？

