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

  1. Java 语言是面向对象的(oop) 

  2. Java 语言是健壮的。Java的强类型机制、异常处理、垃圾的自动收集等是Java程序健壮性的重要保证

  3. Java 语言是跨平台性的。[即: 一个编译好的.class 文件可以在多个系统下运行，这种特性称为跨平台],jvm

  4. Java 语言是解释型的[了解] 

     解释性语言：javascript,PHP, java 

     编译性语言:c/c++ 

     区别是：解释性语言，编译后的代码，不能直接被机器执行,需要解释器来执行, 编译性语言, 编译后的代码, 以直接被机器执行,c/c++

- JVM是一个虚拟的计算机，具有指令集并使用不同的存储区域。负责执行指令，管理数据、内存、寄存器，包含在jdk中，javac,java 编译运行

- JDK 的全称(JavaDevelopment Kit Java 开发工具包) 

  JDK =JRE+java 的开发工具 [java,javac,javadoc,javap 等] 

   JDK是提供给Java开发人员使用的，其中包含了java的开发工具，也包括了JRE。所以安装了JDK，就不用在单独 安装JRE了。

- JRE(Java Runtime Environment Java 运行环境) 

  JRE =JVM+Java 的核心类库[类] 

  包括Java虚拟机(JVMJavaVirtual Machine)和 Java 程序所需的核心类库等，如果想要运行一个开发好的Java程序， 计算机中只需要安装JRE即可。

   JDK、JRE 和 JVM的包含关系 

  1 JDK=JRE+ 开发工具集（例如Javac,java编译工具等)

  2JRE=JVM+JavaSE标准类库（java核心类库）

  3 如果只想运行开发好的 .class文件 只需要JRE

- ![image-20240716195800715](D:/Blog/source/_posts/杂题结论/image-20240716195800715-1721470037252-1.png)

- .java->.class(字节码)->结果

- :question:注意事项：

  一个源代码文件只能有一个public类，其他不限，main也可以写其他里。

  ![image-20240716200450316](D:/Blog/source/_posts/杂题结论/image-20240716200450316-1721470037253-2.png)

- 快速学习技术

- ![image-20240716201023499](D:/Blog/source/_posts/杂题结论/image-20240716201023499-1721470037253-3.png)

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

    ![image-20240716203102795](D:/Blog/source/_posts/杂题结论/image-20240716203102795-1721470037253-5.png)

- 注释comment

  单行注释 // 

  多行注释 /**/ 不允许嵌套

  文档注释 /** */ 可以被javadoc解析

- 代码规范

  ![image-20240716203518265](D:/Blog/source/_posts/杂题结论/image-20240716203518265-1721470037253-4.png)

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

  2024.07.16完成6.813%

## 第04章 运算符(P063 - P103)

- 算数，赋值，关系，逻辑，位，三元运算符

- 算数：+，-，*，/%，++，--，+字符串相加

- a%b=a-a/b*b;

- 关系：==,!=，<.>,>=,<=

- 逻辑:&&,||,!,&,|,^

  ![image-20240717215852723](D:/Blog/source/_posts/杂题结论/image-20240717215852723-1721470037253-6.png)

- 短路效率高

- 赋值：+= ，-= ，*= ， /= ，%= 等

- 三元：条件表达式?表达式1:表达式2; 

- 运算规则： 1.如果条件表达式为true，运算后的结果是表达式1；

  2.如果条件表达式为false，运算后的结果是表达式2；

- 标识符

  ![image-20240717220228776](D:/Blog/source/_posts/杂题结论/image-20240717220228776-1721470037253-8.png)

- 包名：多单词组成时所有字母都小写：aaa.bbb.ccc//比如 com.hsp.crm 

  类名、接口名：多单词组成时，所有单词的首字母大写：XxxYyyZzz[大驼峰] 比如： TankShotGame

   变量名、方法名：多单词组成时，第一个单词首字母小写，第二个单词开始每个单词首字母大写：xxxYyyZzz [小 驼峰， 简称 驼峰法] 比如： tankShotGame 

  常量名：所有字母都大写。多单词时每个单词用下划线连接：XXX_YYY_ZZZ 比如 ：定义一个所得税率 TAX_RATE

  后面我们学习到 类，包，接口，等时，我们的命名规范要这样遵守,更加详细的看文档

- 关键字

  ![image-20240717220438451](D:/Blog/source/_posts/杂题结论/image-20240717220438451-1721470037253-7.png)

  ![image-20240717220451206](D:/Blog/source/_posts/杂题结论/image-20240717220451206-1721470037253-9.png)

- 位运算：>>,<<,>>>,&,|,~,^

- 优先级	运算符	结合性
  1	( )　[ ] 　.	从左到右
  2	! 　~　 ++　 –	从右到左
  3	*　 /　 %	从左到右
  4	+　 -	从左到右
  5	<< 　>>　 >>>	从左到右
  6	< 　<=　 > 　>=　 instanceof	从左到右
  7	== 　!=	从左到右
  8	&	从左到右
  9	^	从左到右
  10	|	从左到右
  11	&&	从左到右
  12	||	从左到右
  13	? :	从左到右
  14	= 　+= 　-= 　*=　 /=　 %=　 &=　 |=　 ^=　 ~= 　<<= 　>>=　 >>>=	从右到左
  15	，	从右到左

- 进制，二，十，八，十六=>0b 0101, ，0，0x or 0X

  各种进制转换：

  1.二，八，十六--->十

  规则：从最低位(右边)开始，将每个位上的数提取出来，乘以2，8，16的(位数-1)次方，然后求和。

  2.十进制--->二，八，十六

  规则：将该数不断除以2，8，16，直到商为0为止，然后将每步得到的余数倒过来，就是对应的二进制。

  3.二--->八，十六

  规则：从低位开始,将二进制数每三，四位一组，转成对应的八，十六进制数即可。

  4.八-->二，十六

  规则：将八进制数每1位，转成对应的一个3位的二进制数即可

  从低位开始，每两位一组，转成对应十六进制。

  5.十六-->二，八

  规则：将十六进制数每1位，转成对应的4位的一个二进制数即可，2位的八进制。

- 原码，反码，补码，（移码）

  负数各位取反+1；计算机都是补码运算

2024.07.17 完成11.318%

比如，封装，继承，多态。。。核心就是减少代码，既然要减少是不是就要封装，那我总不能都封在一个类中啊，那就有了继承，继承多了，我怎么知道谁是老大，那就有了多态。。像[![img](https://i0.hdslb.com/bfs/reply/9f3ad0659e84c96a711b88dd33f4bc2e945045e0.png)自动拆箱](https://search.bilibili.com/all?from_source=webcommentline_search&keyword=自动拆箱&seid=7014867308660033105)，封箱，就是java设计者的弥补，他说了是一切皆对象，那这个基本类型是啥意思，所以后来就出现了这个

## 第05章 程序控制结构(P104 - P155)

- 在程序中，程序运行的流程控制决定程序是如何执行的，是我们必须掌握的，主要有三大流程控制语句。 1) 顺序控制 2) 分支控制 3) 循环控制

- ```java
  if(){};
  
  if(){;}
  else{;}
  
  if()
  else
  if()
  else
  if()
  else
      
  if(){
      if()
      {
          if()else
      }
      else
  }
  else
  ```

  - ```java
    switch(byte,short,int,char,enum[],String){
    case 常量1:
    语句块;
    break;
    case 常量2:
    语句块;
    break;
    default:
    语句块;
    break;
    }//注意匹配了就break，没写break；case穿透就顺序执行直到遇到break;
    ```

- ```java
  for(初始化;循环条件;迭代){循环操作;}
  while(循环条件){
      语句；
      迭代；
  }
  do{
      语句；
      迭代；
  }while(循环条件);
  //多重循环控制
  break;continue;return;
  ```

  ![image-20240718175056646](D:/Blog/source/_posts/杂题结论/image-20240718175056646-1721470037253-10.png)

a:97,A:65

## 第06章 数组、排序和查找(P156 - P191)

- 数组可以存放多个同一类型的数据。数组也是一种数据类型，是引用类型。

- ```java
  //动态初始化
  int a[];orint[]a;
  a=new int[10];
  int a[]=new int[5];
  //静态初始化
  double[]hens={3,5,1,2,88.8};
  int a[]=new int[3]{1,2,3}//error
  int a[]=new int[]{1,2,3};
  ```

  - ![image-20240718181309759](D:/Blog/source/_posts/杂题结论/image-20240718181309759-1721470037253-11.png)

  - 数组是地址，引用传递会变；

  - 就想得到一个不会影响之前的数组：数组拷贝：遍历

  - 数组反转：逆序遍历或者头尾交换、

  - 数组扩容：定义新数组

  - 排序

  - 排序是将多个数据，依指定的顺序进行排列的过程。 

  - 排序的分类： 1内部排序: 指将需要处理的所有数据都加载到内部存储器中进行排序。包括(交换式排序法、选择 式排序法和插入式排序法)； .2外部排序法： 数据量过大，无法全部加载到内存中，需要借助外部存储进行排序。包括(合并排序法和直接合并排序法)。

    ```java
    //冒泡排序
    
    public class BubbleSort{
    
    	public static void main(String[]args){
    		int[] arr={24,69,80,57,12};
            int t=0;
            for(int i=0;i<arr.length;i++){
            	for(int j=0;j<arr.length-1;j++){
            		if(arr[j]>arr[j+1]){t=arr[j];arr[j]=arr[j+1];arr[j+1]=t;}
            	}
            	System.out.print("\n==第"+(i+1)+"轮==");
            	for(int j=0;j<arr.length;j++){
            		System.out.print(arr[j]+"\t");
            	}
            }
    
    	}
    }
    
    ```

  - 查找：顺序，二分。

  - 多维数组-二维数组

  - ```java
    1)语法:类型[][]数组名=new类型[大小][大小]
    2)比如:int a[][]=new int[2][3]
        
    先声明：类型 数组名[][]; 
    再定义(开辟空间) 数组名 =new 类型[大小][大小]
    赋值(有默认值，比如int 类型的就是0)
    
    定义类型数组名[][] ={{值1,值2..},{值1,值2..},{值1,值2..}}
    使用即可[固定方式访问]
    比如:
     int[][]arr={{1,1,1},{8,8,9},{100}};
    int []a,b[];
    b是二维数组,a是一维数组
    ```

    - 注意细节
    - 1)一维数组的声明方式有: int[]x或者intx[] 
    - 2)二维数组的声明方式有: int[][]y或者int[]y[]或者int y[][] 
    - 3)二维数组实际上是由多个一维数组组成的，它的各个一维数组的长度可以相同，也可以不相同。比如：map[][]是 一个二维数组 int map[][]={{1,2},{3,4,5}} 由map[0]是一个含有两个元素的一维数组，map[1]是一个含有三个元素的一维数组构成，我们也称为列数不等的二维数组

  2024.07.18 完成20.989%

## 第07章 面向对象编程（基础部分）(P192 - P263)

- 为什么要用面向对象就是要便与数据的管理和提高效率

- 用变量太多太麻烦，用数组也体现不出数据类型，只能通过下标获取，不能体现行为

- 封装，继承，多态

- 一个程序就是一个世界，有很多事物(对象[属性, 行为])

- ![image-20240719231202537](D:/Blog/source/_posts/杂题结论/image-20240719231202537-1721470037253-14.png)

- 我上早八，我吃柠檬的

- 类和对象的区别与联系

  1) 类是抽象的，概念的，代表一类事物,比如人类,猫类.., 即它是数据类型. 
  2) 对象是具体的，实际的，代表一个具体事物, 即 是实例. 
  3) 类是对象的模板，对象是类的一个个体，对应一个实例

- 对象在内存中的存在形式：

  堆：对象 栈：基本数据方法区：字符串

  ![image-20240720101631122](D:/Blog/source/_posts/杂题结论/image-20240720101631122-1721470037253-12.png)

- 属性/成员变量/字段

  1) 从概念或叫法上看： 成员变量 = 属性 =field(字段) 
  2) 属性是类的一个组成部分，一般是基本数据类型,也可是引用类型(对象，数组)。比如我们前面定义猫类的int age就 是属性。

- 注意：

  1.属性的定义语法同变量，示例：访问修饰符属性类型属性名; 这里老师简单的介绍访问修饰符：控制属性的访问范围 有四种访问修饰符public,proctected,默认,private,

  2.属性的定义类型可以为任意类型，包含基本类型或引用类型 

  3.属性如果不赋值，有默认值，规则和数组一致。具体说:int 0，short0,byte0,long0,float0.0,double0.0，char\u0000，booleanfalse，Stringnull

- ```java
  //如何创建对象
  1) 先声明再创建
  Cat cat ; //声明对象 cat
   cat = new Cat(); //创建
  2) 直接创建
  Cat cat = new Cat();
   如何访问属性
   基本语法
  对象名.属性名;
  案例演示赋值和输出
  cat.name ;
   cat.age;
   cat.color;
  //1.在方法区加载类信息：属性和行为（方法）信息
  //2.在堆开空间还是默认值
  //3.堆到栈就有了地址是对应类名字
  //4.放东西分配空间
  ```

- 成员方法:在某些情况下，我们要需要定义成员方法(简称方法)。比如人类:除了有一些属性外(年龄，姓名..),我们人类还有一 些行为比如:可以说话、跑步..,通过学习，还可以做算术题。这时就要用成员方法才能完成。

- ```java
  访问修饰符返回数据类型方法名（形参列表..）{//方法体
  语句；
  return返回值;
   }
  1)提高代码的复用性
  2)可以将实现的细节封装起来，然后供其他用户来调用即可
  ```

- ![image-20240720110528839](D:/Blog/source/_posts/杂题结论/image-20240720110528839-1721470037253-13.png)

- ![image-20240720110649088](D:/Blog/source/_posts/杂题结论/image-20240720110649088-1721470037253-17.png)

- ![image-20240720110701224](D:/Blog/source/_posts/杂题结论/image-20240720110701224-1721470037253-15.png)

- 注意地址，值传递和引用传递。

- 递归调用：

  递归就是方法自己调用自己,每次调用时传入不同的变量.递归有助于编程者解决复杂问题,同时可以让代码变 得简洁

  ![image-20240720115058601](D:/Blog/source/_posts/杂题结论/image-20240720115058601-1721470037253-16.png)

- 迷宫，汉诺塔，八皇后

  ```java
  public class Hello{
  
  	public static void main(String[]args){
         int[][] map =  new int[8][7];
         for(int i=0;i<7;i++){
         	map[0][i]=1;map[7][i]=1;
         }
         for(int i=0;i<8;i++){
         	map[i][0]=1;map[i][6]=1;
         }
         map[3][1]=1;map[3][2]=1;map[1][5]=1;
         T p =new T();
         p.findWay(map,1,1);
         System.out.println("====当前地图情况====");
         for(int i=0;i<map.length;i++){
         	for(int j=0;j<map[i].length;j++){
         		System.out.print(map[i][j]+" ");
         	}
         	System.out.println();
         }
  	}
  }
  
  class T{
  		public boolean findWay(int[][] map,int i,int j){
            if(map[6][5]==2)return true;
            else{
            	if(map[i][j]==0){
                 map[i][j]=2;
                 if(findWay(map,i-1,j)){
                 	return true;
                 }else if(findWay(map,i,j+1)){
                   return true;
                 }else if(findWay(map,i+1,j)){
                 	return true;
                 }else if(findWay(map,i,j-1)){
                 	return true;
                 }else {map[i][j]=3;return false;}
            	}
            	else{
            		return false;
            	}
            }
  		}
  }
  
  //汉诺塔
  public class Hello{
  
  	public static void main(String[]args){
        T p=new T();
        p.move(3,'A','B','C');
  	}
  }
  
  class T{
  		public void move(int num,char a,char b,char c){
  			if(num==1){
  				System.out.println(a+"->"+c);
  			}else{ //如果有多个盘，可以看成两个,最下面的和上面的所有盘(num-1)
   //(1)先移动上面所有的盘到b,借助c
  				move(num-1,a,c,b);
  				 //(2)把最下面的这个盘，移动到c
  				System.out.println(a+"->"+c);
  				 //(3)再把b塔的所有盘，移动到c,借助a
                  move(num-1,b,a,c);
  			}
  		}
  }
  //八皇后
  
  ```

  

- 重载（overload)

  java 中允许同一个类中，多个同名方法的存在，但要求 形参列表不一致！

- 可变参数

  java允许将同一个类中多个同名同功能但参数个数不同的方法，封装成一个方法。 就可以通过可变参数实现

  ```java
  访问修饰符 返回类型 方法名(数据类型...形参名){
   }
  public class VarParameter01 {
   //编写一个main方法
  public static void main(String[] args) {
   HspMethod m = new HspMethod();
   System.out.println(m.sum(1, 5, 100)); //106
   System.out.println(m.sum(1,19)); //20
   }
   }
   class HspMethod {
   //可以计算 2个数的和，3个数的和 ， 4.5， 。。
  //可以使用方法重载
  // public int sum(int n1, int n2) {//2 个数的和
  //
   // }
   return n1 + n2;
   // public int sum(int n1, int n2, int n3) {//3 个数的和
  //
   // }
   //
   return n1 + n2 + n3;
   return n1 + n2 + n3 + n4;
   // public int sum(int n1, int n2, int n3, int n4) {//4 个数的和
  // }
   //.....
   //上面的三个方法名称相同，功能相同, 参数个数不同-> 使用可变参数优化
       //1.int...表示接受的是可变参数，类型是int,即可以接收多个int(0-多)
   //2.使用可变参数时，可以当做数组来使用即nums可以当做数组
  //3.遍历nums求和即可
  public int sum(int...nums){
   //System.out.println("接收的参数个数="+nums.length);
   int res=0;
   for(int i=0;i<nums.length;i++){
   res+=nums[i];
   }
   return res;
   }
   }
  ```

  ![image-20240720184838701](D:/Blog/source/_posts/杂题结论/image-20240720184838701.png)

- 作用域（scope)

  ![image-20240720205037904](D:/Blog/source/_posts/杂题结论/image-20240720205037904.png)

  ![image-20240720205057498](D:/Blog/source/_posts/杂题结论/image-20240720205057498.png)

- 构造方法/构造器

- 直接指定属性值等

  [修饰符] 方法名(形参列表){ 方法体; }

    老韩说明： 1) 构造器的修饰符可以默认， 也可以是public protected private 2) 构造器没有返回值 3) 方法名 和类名字必须一样 4) 参数列表 和 成员方法一样的规则 5) 构造器的调用, 由系统完成

- 构造方法又叫构造器(constructor)，是类的一种特殊的方法，它的主要作用是完成对**新对象的初始化**。它有几个特点：1)方法名和类名相同 2) 没有返回值   3) 在创建对象时，系统会自动的调用该类的构造器完成对象的初始化。

  ![image-20240720215436354](D:/Blog/source/_posts/杂题结论/image-20240720215436354.png)

```java

public class Hello{

	public static void main(String[]args){
	 Person p =new Person("king",40);
	 Person p =new Person("tom");
	}
}

class Person{
     String name;
     int age;
     //第一个构造器
     public Person(String pName,int pAge){
     	name = pName;
     	age = pAge;
     }
     //第二个构造器
     public Person(String pName){
     	name = pName;
     }
}
//javap -c/v
```

- 对象创建流程分析

- ![image-20240721144056434](D:/Blog/source/_posts/杂题结论/image-20240721144056434.png)

- ![image-20240721144133623](D:/Blog/source/_posts/杂题结论/image-20240721144133623.png)

- this

  解决方法赋值/变量命名问题：

  ```java
  
  public class Hello{
  
  	public static void main(String[]args){
  	 Person p =new Person("king",40);
  	 Person p1=new Person("tom");
  	}
  }
  
  class Person{
       String name;
       int age;
       //第一个构造器
       
       //第二个构造器
       public Person(String pName){
       	name = pName;
       }
       public Person(String name,int age){
       	this.name = name;
       	this.age = age;
       }
  }
  ```

- this 的本质：

  从内存上讲：

  ![image-20240722151233603](D:/Blog/source/_posts/杂题结论/image-20240722151233603.png)

-  this 的注意事项和使用细节

  1) this 关键字可以用来访问本类的属性、方法、构造器

  2)   this 用于区分当前类的属性和局部变量 

  3)  访问成员方法的语法：this.方法名(参数列表);下一步继承讲

  4) 访问构造器语法：this(参数列表);注意只能在构造器中使用(即只能在构造器中访问另外一个构造器,必须放在第一 条语句)

  5) this不能在类定义的外部使用，只能在类定义的方法中使用。就近原则找不用this时。

     ```java
     public class TestPerson{
      //编写一个main方法
     public static void main(String[]args){
      Person p1=new Person("mary",20);
      Person p2=new Person("mary",20);
      System.out.println("p1和p2比较的结果="+p1.compareTo(p2));
      }
      }
      class Person{
      String name;
      int age;
      //构造器
     public Person(String name,int age){
      this.name=name;
      this.age=age;
      }
      //compareTo比较方法
     public boolean compareTo(Person p){
      //名字和年龄完全一样
     //if(this.name.equals(p.name)&&this.age==p.age){
      // return true;
      //}else{
      // return false;
      //}
      return this.name.equals(p.name)&&this.age==p.age;
      }
      }
     //equals()和==:
     /*在Java编程语言中，equals和==是两种不同的比较操作。
     
     ==操作符：
     对于基本数据类型（如int、float、char等），==比较的是两个变量的值是否相等。
     对于引用数据类型（如Object、数组、类实例等），==比较的是两个引用是否指向内存中的同一个对象，即它们是否引用相同的内存地址。
     equals方法：
     equals是Object类中的一个方法，可以被继承和重写。在默认的实现中，即Object类中的equals方法，它与==操作符的行为是一样的，比较的是引用是否相同。
     但是，对于许多Java类库中的类（如String、Integer、Date等），equals方法被重写以比较对象的实际内容是否相等，而不是它们的引用。*/
     String s1 = new String("Hello");
     String s2 = new String("Hello");
     
     // 使用 == 比较
     System.out.println(s1 == s2); // 输出 false，因为它们是不同的对象实例
     
     // 使用 equals 方法比较
     System.out.println(s1.equals(s2)); // 输出 true，因为它们的内容相同
     
     ```

     匿名对象只能用一次后被销毁。

2024.07.22 完成30.549%到包

## 第08章 面向对象编程（中级部分）(P264 - P361)

- IDEA（集成开发环境）

  1) 删除当前行, 默认是ctrl+Y 自己配置 ctrl+d

  2)  复制当前行, 自己配置 ctrl+alt+ 向下光标 

  3) 补全代码 alt+/ 

  4) 添加注释和取消注释 ctrl+/ 【第一次是添加注释，第二次是取消注释】

  5)  导入该行需要的类 先配置auto import, 然后使用 alt+enter即可 

  6)  快速格式化代码 ctrl+alt+L 

  7)  快速运行程序 自己定义 alt+R 

  8) 生成构造器等 alt+insert [提高开发效率] 

  9)  查看一个类的层级关系 ctrl+H [学习继承后，非常有用]

  10)  自动的分配变量名 , 通过 在后面假 .var [老师最喜欢的] 

  11)  还有很多其它的快捷键...  

  12)  将光标放在一个方法上，输入 ctrl+B, 可以定位到方法 [学继承后，非常有用

      模板的自定义

- 包

  ![image-20240722223454369](D:/Blog/source/_posts/杂题结论/image-20240722223454369.png)

- ![image-20240722223546071](D:/Blog/source/_posts/杂题结论/image-20240722223546071.png)

- ![image-20240722223658540](D:/Blog/source/_posts/杂题结论/image-20240722223658540.png)

- 访问修饰符

  ![image-20240722223728110](D:/Blog/source/_posts/杂题结论/image-20240722223728110.png)

- 封装

  面向对象编程有三大特征：封装、继承和多态.

  封装（encapsulation)就是把抽象出的数据[属性]和对数据的操作【方法】封装在一起，数据被保护在内部，程序的其他部分只有通过被授权的操作【方法】，才能对数据进行操作。

  理解和好处：

  ```java
  1）隐藏实现细节：方法（连接数据库）<--调用（传入参数。。）
  2）可以对数据进行验证，保证安全合理
  Person {name,age}
  Person p =  new Person();
  p.name = "jack";
  p.age = 1200;
  ```

  实现步骤(三步走)

  >1）将属性进行私有化private【不能直接修改属性】
  >
  >2）提供一个公共的（public）set方法，用于对属性判断并赋值
  >
  >public void setXXX(类型 参数名){//XXX 表示某个属性
  >
  >//加入数据验证的业务逻辑
  >
  >属性=参数名；
  >
  >}
  >
  >3）提供一个公共的（public）get方法，用于获取属性的值
  >
  >public 数据类型 getXxx{//权限判断，Xxx某个属性
  >
  >return xx;
  >
  >}

  入门案例

  ```java
  public class Test {
      public static void main(String[] args) {
          // TODO Auto-generated method stub
          MyTools mt = new MyTools();
          mt.setName("jacksss");
          mt.setAge(18);
          mt.setSalary(30000);
          System.out.println(mt.info());
      }
  }
  
  class MyTools {
      public String name;
      private int age;
      private double salary;
      //自己写get，set太慢快捷键
      public MyTools(String name, int age,double salary){
          //this.name = name;
         // this.age = age;
          //this.salary = salary;
          setName(name);
          setAge(age);
          setSalary(salary);
      }//写构造器就绕过了set方法，解决：写到构造器里
      public String getName() {
          return name;
      }
  
      public void setName(String name) {
          if(name.length()>=2&&name.length()<=6){
              this.name = name;
          }else{
              System.out.println("名字长度不对，需要2-6个字符");
              this.name = "ss";
          }
      }
  
      public int getAge() {
          return age;
      }
  
      public void setAge(int age) {
          if(age >=1&&age<=120) {
              this.age = age;
          }else{
              System.out.println("你设置的年龄不对，需要在1-120之间");
              this.age = 18;
          }
      }
  
      public double getSalary() {
          return salary;
      }
  
      public void setSalary(double salary) {
          this.salary = salary;
      }
      public String info(){
          return "信息为 name="+name +" age"+age+" 薪水"+salary;
      }
  } //end of class
  ```

  

  2024.07.25 完成31.378到封装

- 继承

  目的：提高代码复用性,代码的扩展性和维护性提高。

  ![image-20240726163628171](D:/Blog/source/_posts/杂题结论/image-20240726163628171.png)

  ```java
  语法：
  class 子类 extends 父类{
  }
  1)子类会自动拥有父类定义的属性以及方法；
  2）父类又叫超类，基类；
  3）子类又叫派生类。
  ```

  >继承的深入讨论/细节问题
  >
  > 1.子类继承了所有的属性和方法，非私有的属性和方法可以在子类直接访问,但是私有属性和方法不能在子类直接访 问，要通过父类提供公共的方法去访问 
  >
  >2.子类必须调用父类的构造器，完成父类的初始化 
  >
  >3.当创建子类对象时，不管使用子类的哪个构造器，默认情况下总会去调用父类的无参构造器，如果父类没有提供无参构造器，则必须在子类的构造器中用super去指定使用父类的哪个构造器完成对父类的初始化工作，否则，编译不会通过（怎么理解。）举例说明
  >
  >```java
  >super(参数)父类的
  >    //
  >this()指的是在构造器里调用另外一个构造器。自己的
  >```
  >
  >4.如果希望指定去调用父类的某个构造器，则显式的调用一下:super(参数列表) 5. super在使用时，必须放在构造器第一行(super只能在构造器中使用)
  >
  >6.super()和this()都只能放在构造器第一行，因此这两个方法不能共存在一个构造器 .
  >
  >7.java所有类都是Object类的子类,Object是所有类的基类.
  >
  >8.父类构造器的调用不限于直接父类！将一直往上追溯直到Object类(顶级父类) 
  >
  >9.子类最多只能继承一个父类(指直接继承)，即java中是单继承机制。 思考：如何让A类继承B类和C类？【A继承B，B继承C】 
  >
  >10.不能滥用继承，子类和父类之间必须满足is-a的逻辑关系

  

  super()自动调用父类的无参构造器//没有就是隐含着

  继承的本质：在jvm内存里的调用执行

  ![image-20240727170037955](D:/Blog/source/_posts/杂题结论/image-20240727170037955.png)

  2024.07.26 完成32.637%到继承

- super

  super代表父类的引用，用于访问父类的属性、方法、构造器.

  > 1.访问父类的属性，但不能访问父类的private属性 super.属性名
  >
  > 2.访问父类的方法，不能访问父类的private方法 super.方法名（参数列表）
  >
  > 3.访问父类的构造器 super.（参数列表）只能放在第一行

  ![image-20240727004504386](D:/Blog/source/_posts/杂题结论/image-20240727004504386.png)

- override方法重写/覆盖

  简单的说：方法覆盖（重写）就是子类有一个方法，和父类的某个方法的名称，返回类型，参数一样，那么我们就说子类的这个方法覆盖了父类的方法。

  > 注意细节：
  >
  > 1.子类的方法的形参列表，方法名称，要和父类方法的形参列表，方法名称完全一样。
  >
  > 2.子类方法的返回类型和父类的返回类型一样，或者是父类返回类型的子类。
  >
  > 比如 父类 返回类型是Object，子类方法返回类型是String。这是在到顶级父类时
  >
  > 3.子类方法不能缩小父类方法的访问权限 public> protected>默认>private;

  ![image-20240727225607080](D:/Blog/source/_posts/杂题结论/image-20240727225607080.png)

  2024.07.27 完成33.516%到override

  

  - 多态polymorphic

  要操作的很多不利于维护和管理，写很多一样的。

  传统的方法带来的问题是什么?

  如何解决? 问题是：代码的复用性不高，而且不利于代码维护

   解决方案：引出我们要讲解的多态

  **方法或对象具有多种形态。是面向对象的第三大特征，多态是建立在封装和继承基础之上的。**

  方法重载和重写体现多态

  ```java
  Animal animal = new Dog();
  animal.cry();
  animal = new  Cat();
  animal.cry();
  Cat cat =(Cat)animal;
  cat instanceof Animal//boolen值
  ```

  对象的多态：

  > 1.一个对象的编译类型和运行类型可以不一致
  >
  > 2.编译类型在定义对象时，就确定了，不能改变
  >
  > 3.运行类型是可以变化的 getClass
  >
  > 4.编译类型是看定义时 = 号的左边，运行类型看 = 号的右边。就可以变了，关键是减少代码量
  >
  > 5.属性没有重写一说就是找编译类型的属性
  >
  > 6.instanceof :判断某某对象的运行类型是否为xx类型或xx类型的子类型

  ![image-20240728182035917](D:/Blog/source/_posts/杂题结论/image-20240728182035917.png)

  :star:java的动态绑定机制

  ![image-20240728182140190](D:/Blog/source/_posts/杂题结论/image-20240728182140190.png)

​       DynamicBinding:方法就得调用运行类型的，属性不需要。

多态的应用

多态数组：

数组的定义为父类类型，里面保存的实际元素为子类类型

```java
Person[] persons = new Person[5];
persons[0]=new Person();
persons[1]=new Student();
persons[2]=new Teacher();
for(int i=0;i<persons.length;i++){
    if(persons[i]instanceof Student){//判断运行类型是否为Student
        Student student=(Student)persons[i];
        student.study();
        //((Student)persons[i].study());
    }
}
```

多态参数:

方法定义的形参类型为父类类型，实参类型允许为子类类型

```java
package com.polyparameter;

public class Ployparameter {
    public static void main(String []args){
        Worker tom = new Worker("tom", 2500.0);
        Manger milan = new Manger("milan", 5000.0,200000);
        Ployparameter ployparameter = new Ployparameter();
        ployparameter.showEmpAnnual(tom);
        ployparameter.showEmpAnnual(milan);
        ployparameter.testWork(tom);
        ployparameter.testWork(milan);
    }
    public void showEmpAnnual(Employee e){
        System.out.println(e.getAnnual());
    }
    public void testWork(Employee e){
        if(e instanceof Worker){
            ((Worker)e).work();
        }else if(e instanceof Manger){
            ((Manger)e).mange();
        }else{
            System.out.println("不做处理...");
        }
    }
}

```

千万不要眼高手低。2024.07.28 完成34.945%

- object类

  equals:

  ![image-20240728232125668](D:/Blog/source/_posts/杂题结论/image-20240728232125668.png)

  如何重写equals方法：

  ```java
  public boolean equals(Object anObject) {
          if (this == anObject) {
              return true;
          }
          if (anObject instanceof String) {
              String anotherString = (String)anObject;
              int n = value.length;
              if (n == anotherString.value.length) {
                  char v1[] = value;
                  char v2[] = anotherString.value;
                  int i = 0;
                  while (n-- != 0) {
                      if (v1[i] != v2[i])
                          return false;
                      i++;
                  }
                  return true;
              }
          }
          return false;
      }
  Object 的就是:
  public boolean qauals(Object anObject){
      return this == anObject;
  }
   public boolean equals(Object obj) {
          if (obj instanceof Integer) {
              return value == ((Integer)obj).intValue();
          }
          return false;
      }
  
  
    public boolean equals(Object p){
          if(this == p)return true;
          if(p instanceof Person){
              //向下转型
              Person q = (Person) p;
              return this.name.equals(q.name)&&this.age==q.age&&this.gender==q.gender;
          }
          return false;
      }
  ```

  hashCode:返回该对象的哈希码值，支持此方法是为了提高哈希表的性能。

  > 1)提高具有哈希结构的容器的效率！
  >
  > 2)两个引用，如果指向的是同一个对象，则哈希值肯定是一样的！ 
  >
  > 3)两个引用，如果指向的是不同对象，则哈希值是不一样的 
  >
  > 4)哈希值主要根据地址号来的！， 不能完全将哈希值等价于地址。
  >
  > 5)案例演示[HashCode_.java]:obj.hashCode() [测试：A obj1=new A();A obj2=new A();A obj3=obj1] 
  >
  > 6)后面在集合，中hashCode如果需要的话，也会重写,在讲解集合时，老韩在说如何重写hashCode()
  >
  > ```java
  >  public class HashCode_{
  >  public static void main(String[]args){
  >  AA aa=new AA();
  >  AA aa2=new AA();
  >  AA aa3=aa;
  >  System.out.println("aa.hashCode()="+aa.hashCode());
  >  System.out.println("aa2.hashCode()="+aa2.hashCode());
  >  System.out.println("aa3.hashCode()="+aa3.hashCode());
  >  }
  >  }
  >  classAA{}
  > ```
  >
  > 

  toString:

  1)基本介绍 默认返回：全类名(包名加类名）+@+哈希值的十六进制，【查看Object的toString方法】 子类往往重写toString方法，用于返回对象的属性信息 

  ```java
      public String toString() {
          return getClass().getName() + "@" + Integer.toHexString(hashCode());
      }
  ```

  2)重写toString方法，打印对象或拼接对象时，都会自动调用该对象的toString形式

  案例演示：Monster[name,job, sal] 案例:ToString_.java 

  3）当直接输出一个对象时，toString 方法会被默认的调用, 比如 System.out.println(monster)； 就会默认调用 monster.toString()

  finalize:

  1)当对象被回收时，系统自动调用该对象的finalize方法。子类可以重写该方法，做一些释放资源的操作【演示】

   2)什么时候被回收：当某个对象没有任何引用时，则jvm就认为这个对象是一个垃圾对象，就会使用垃圾回收机制来 销毁该对象，在销毁该对象前，会先调用finalize方法。 

  3)垃圾回收机制的调用，是由系统来决定(即有自己的GC算法),也可以通过System.gc()主动触发垃圾回收机制，测 试：Car[name]

   老韩提示：我们在实际开发中，几乎不会运用finalize,所以更多就是为了应付面试.

  getClass:在 Java 中，`getClass()` 是一个方法，用于获取对象的运行时类。这个方法属于 `Object` 类，因此所有 Java 对象都可以调用它。

  使用 `getClass()` 方法的基本语法如下：

  ```java
  Class<?> class_name = object.getClass();
  public class MyClass {
      public static void main(String[] args) {
          MyClass obj = new MyClass();
          Class<?> class_name = obj.getClass();
  
          System.out.println(class_name);  // 输出：class MyClass
      }
  }
  ```

  

- 断点调试(debug)

  ![image-20240729224627340](D:/Blog/source/_posts/杂题结论/image-20240729224627340.png)

force step into 进入 alt+shift+f7 or

Debugger java.* 和javax.*

零钱通项目：使用Java 开发 零钱通项目 , 可以完成收益入账，消费，查看明细，退出系统等功能.

化繁为简. 1) 先完成显示菜单，并可以选择 2) 完成零钱通明细. 3) 完成收益入账 4) 消费 5) 退出

```java
package com.smallcahnge;

import java.text.SimpleDateFormat;
import java.util.Date;
import java.util.Scanner;

public class SmallChangeSys {
    public static void main(String []args){
        boolean loop = true;
        Scanner scanner = new Scanner(System.in);
        String key="";
        String details = "-------------零钱通明细----------";
        double money = 0;
        double balance = 0;
        Date date = null;
        String note;
        SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd HH:mm");

        do{
            System.out.println("\n=============零钱通菜单=============");
            System.out.println("\t\t\t1 零钱通明细");
            System.out.println("\t\t\t2 收益入账");
            System.out.println("\t\t\t3 消费");
            System.out.println("\t\t\t4 退    出");
            System.out.print("请选择（1-4）： ");
            key=scanner.next();
            switch (key){
                case "1":
                    System.out.println(details);
                    break;
                case "2":
                    System.out.print("收益入账金额：");
                    money = scanner.nextDouble();
                    if(money<=0){
                        System.out.println("收益入账金额 需要  大于 0");
                        break;
                    }
                    balance+=money;
                    date = new Date();
                    details+="\n收益入账\t+"+money+"\t"+sdf.format(date)+"\t"+balance;
                    break;
                case "3":
                    System.out.print("消费金额:");
                    money =scanner.nextDouble();
                    if(money<=0||money>balance){
                        System.out.println("你的消费金额 应该在0-"+balance+"元");
                        break;
                    }
                    System.out.print("消费说明：");
                    note = scanner.next();
                    balance-=money;
                    date=new Date();
                    details+="\n"+note+"\t-"+money+"\t"+sdf.format(date)+"\t"+balance;
                    break;
                case "4":
                    String choice = "";
                    while(true){
                        System.out.println("你确定要退出吗？y/n");
                        choice = scanner.next();
                        if("y".equals(choice)||"n".equals(choice)){
                            break;
                        }
                    }
                    if(choice.equals("y")){
                    loop=false;
                    }
                    break;
                default:
                    System.out.println("菜单选择有误,请重新选择");
            }
        }while(loop);
        System.out.println("------退出了零钱通项目------");
    }
}
```

oop类型

编译类型自己可以写，运行类型是运行中可以用。

Integer 在-127-128之间用==是true;

调用父类有参构造隐藏个super（）；

求悟

2024.07.29 完成39.670%

## 第09章 房屋出租系统(P362 - P373)

分层模式 基本简单的设计模式

房屋租赁程序框架图

1.系统有哪些类/文件，2.明确类与类的调用关系

HouseView.java 1.显示界面2.接受用户的输入3.调用其他类完成对房屋信息的各种操作//界面层

HouseService.java1.响应View的调用2.完成对房屋信息的各种操作（crud增删改查）//业务层

House.java 1.一个House对象表示一个房屋信息//实体类domain/model

HouseRentApp.java 创建对象，调用显示 主程序

工具类 提供服务

<img src="D:/Blog/source/_posts/杂题结论/image-20240731214212745.png" alt="image-20240731214212745" style="zoom: 200%;" />



实现功能的三部曲 [明确完成功能->思路分析->代码实现]

当一个方法是static时，可以通过类名调用

业精于勤，荒于嬉，行成于思，毁于随。

2024.07.31 完成40.989%

