### JAVA EE组 阶段一笔记

#### 一、关于JDK、JRE、JVM

> JDK : Java Development Kit
>
> JRE : Java Runtime Enviroment
>
> JVM : Java Virtual Machine

1. 包含关系

   JDK包含JRE，JRE包含JVM。
   
2. 作用

   * JDK用于用java开发
   * JRE用于运行java编写的程序，如果不开发只运行则仅需JRE而无需JDK
   
   * 不同的平台的JVM是不同的，但是可以实现Java语言在不同平台上运行时不需要重新编译。仅有JVM是无法运行Java程序的。

#### 二、用记事本编写Hello World

~~~java
public class HelloWorld{
    public static void main(String[] args){
        System.out.println("Hello World!");
    }
}
~~~

1. 记事本编写

   ![helloworld0](D:\txy\university\New_Thread\JAVA\笔记\helloworld0.PNG)

2. 试运行

<img src="D:\txy\university\New_Thread\JAVA\笔记\javaEE_tasks\Java_EE_tasks\task1\helloworld.PNG" alt="helloworld" style="zoom: 150%;" /><img src="D:\txy\university\New_Thread\JAVA\笔记\javaEE_tasks\Java_EE_tasks\task1\HelloWorld1.PNG" alt="HelloWorld1" style="zoom:150%;" />

3. 打印中文字符：在编译文件前加入-encoding UTF-8

   代码：

   ```java
   public class 打印中文 {
   	public static void main(String[] args) {
   		System.out.println("你好，世界!");
   	}
   }
   ```

   编译运行：

   ![打印中文](D:\txy\university\New_Thread\JAVA\笔记\javaEE_tasks\Java_EE_tasks\task1\打印中文.PNG)

   

#### 三、用IDEA写Hello World

<img src="D:\txy\university\New_Thread\JAVA\笔记\javaEE_tasks\Java_EE_tasks\task1\helloworld_idea1.PNG" style="zoom:80%;" />



![helloworld_idea2](D:\txy\university\New_Thread\JAVA\笔记\javaEE_tasks\Java_EE_tasks\task1\helloworld_idea2.PNG)

