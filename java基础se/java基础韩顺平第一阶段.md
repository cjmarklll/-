# 第一阶段(养成编程思想)

## 第01章 内容介绍(P001 - P006)

- 开源的思想看世界。。。,基础很重要


- 就业方向：javaEE工程师，大数据软件，Android软件工程...

- 开发场景：ssm🦎:spring,springmvc,mybatis
- 企业级应用，安卓，移动，大数据。
- 再牛的都是小白开始，别人能学会的你也一定能学会。

## 第02章 Java概述(P007 - P034)

- 程序：计算机执行某些操作或解决某个问题而编写的一系列有序指令的集合

- Java技术体系平台

  | Java  se | Java ee | Java me |
  | -------- | ------- | ------- |
  | 桌面级   | 企业级  | 移动    |

- Java 重要特点

  1) Java 语言是面向对象的(oop) 

  2)   Java 语言是健壮的。Java的强类型机制、异常处理、垃圾的自动收集等是Java程序健壮性的重要保证

  3)  Java 语言是跨平台性的。[即: 一个编译好的.class 文件可以在多个系统下运行，这种特性称为跨平台],jvm

  4)   Java 语言是解释型的[了解] 

     解释性语言：javascript,PHP, java 

     编译性语言:c/c++ 

     区别是：解释性语言，编译后的代码，不能直接被机器执行,需要解释器来执行, 编译性语言, 编译后的代码, 以直接被机器执行,c/c++

- JVM是一个虚拟的计算机，具有指令集并使用不同的存储区域。负责执行指令，管理数据、内存、寄存器，包含在jdk中，javac,java 编译运行

- JDK 的全称(JavaDevelopment Kit Java 开发工具包) 

  JDK =JRE+java 的开发工具 [java,javac,javadoc,javap 等] 

   JDK是提供给Java开发人员使用的，其中包含了java的开发工具，也包括了JRE。所以安装了JDK，就不用在单独 安装JRE了。

-  JRE(Java Runtime Environment Java 运行环境) 

  JRE =JVM+Java 的核心类库[类] 

  包括Java虚拟机(JVMJavaVirtual Machine)和 Java 程序所需的核心类库等，如果想要运行一个开发好的Java程序， 计算机中只需要安装JRE即可。

   JDK、JRE 和 JVM的包含关系 

  1 JDK=JRE+ 开发工具集（例如Javac,java编译工具等)

  2JRE=JVM+JavaSE标准类库（java核心类库）

  3 如果只想运行开发好的 .class文件 只需要JRE

- ![image-20240716195800715](D:/Blog/source/_posts/杂题结论/image-20240716195800715.png)

-  .java->.class(字节码)->结果

- :question:注意事项：

  一个源代码文件只能有一个public类，其他不限，main也可以写其他里。

  ![image-20240716200450316](D:/Blog/source/_posts/杂题结论/image-20240716200450316.png)

- 快速学习技术
- ![image-20240716201023499](D:/Blog/source/_posts/杂题结论/image-20240716201023499.png)

-    

  ```
  /*
  \t：一个制表位，实现对齐的功能
  \n ：换行符
  \\：一个\
   \" :一个"
   \'：一个'
   \r:一个回车 System.out.println("韩顺平教育\r 北京")*/
   北京平教育 \r\n
  ```

  - 初学java易犯错误

    ![image-20240716203102795](D:/Blog/source/_posts/杂题结论/image-20240716203102795.png)

- 注释comment

  单行注释 // 

  多行注释 /**/ 不允许嵌套

  文档注释 /** */ 可以被javadoc解析

- 代码规范

  ![image-20240716203518265](D:/Blog/source/_posts/杂题结论/image-20240716203518265.png)

- DOS命令（了解即可）

  Dos： Disk Operating System 磁盘操作系统, 简单说一下windows的目录结构。相对路径和绝对路径

  ```java
  1.查看当前目录是有什么内容 dir 
  dir dir d:\abc2\test200
  2.切换到其他盘下：盘符号 cd:changedirectory 
  案例演示：切换到 c盘 cd/D c: 
  3. 切换到当前盘的其他目录下 (使用相对路径和绝对路径演示), ..\表示上一级目录 
  案例演示： cd d:\abc2\test200 cd..\..\abc2\test200 
  4.切换到上一级： 
  案例演示： cd.. 
  5. 切换到根目录：cd\ 
  案例演示：cd\ 
  6. 查看指定的目录下所有的子级目录 tree 
  7.清屏 cls[苍老师] 
  8. 退出DOS exit 
  说明: 因为小伙伴后面使用DOS 非常少，所以对下面的几个指令，老韩给大家演示下, 大家了解即可 (md[创建目 录],rd[删除目录],copy[拷贝文件]  指定路径,del[删除文件],echo[输入内容到文件]>,type nul>,move[剪切]) => Linux
  ```

  

## 第03章 变量(P035 - P062)

- 变量是程序的基本组成单位 类型+名字=；
- ![image-20240716212808751](D:\Blog\source\_posts\杂题结论\image-20240716212808751.png)

- ![image-20240716214312679](D:\Blog\source\_posts\杂题结论\image-20240716214312679.png)

- ![image-20240716214641412](D:\Blog\source\_posts\杂题结论\image-20240716214641412.png)

- ![image-20240716215315208](D:\Blog\source\_posts\杂题结论\image-20240716215315208.png)

- ![image-20240716215544423](D:\Blog\source\_posts\杂题结论\image-20240716215544423.png)

- javaAPI文档

  ![image-20240716221506406](D:\Blog\source\_posts\杂题结论\image-20240716221506406.png)

- ![image-20240716221847703](D:\Blog\source\_posts\杂题结论\image-20240716221847703.png)
- ![image-20240716222623949](D:\Blog\source\_posts\杂题结论\image-20240716222623949.png)

- ASCIII码

- Boolen类型

- 强制转换和自动转换

  ![image-20240716222934146](D:\Blog\source\_posts\杂题结论\image-20240716222934146.png)

  ![image-20240716222942795](D:\Blog\source\_posts\杂题结论\image-20240716222942795.png)

  - ![image-20240716223013729](D:\Blog\source\_posts\杂题结论\image-20240716223013729.png)

  2024.07.16完成6.8%

## 第04章 运算符(P063 - P103)



## 第05章 程序控制结构(P104 - P155)



## 第06章 数组、排序和查找(P156 - P191)



## 第07章 面向对象编程（基础部分）(P192 - P263)



## 第08章 面向对象编程（中级部分）(P264 - P361)



## 第09章 房屋出租系统(P362 - P373)

