<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [:point_right:java环境变量](#point_rightjava%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F)
  - [:point_right:Java 命令行参数 - 运行java](#point_rightjava-%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0---%E8%BF%90%E8%A1%8Cjava)
  - [:point_right:Javac 命令命令行参数 - 编译java文件](#point_rightjavac-%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0---%E7%BC%96%E8%AF%91java%E6%96%87%E4%BB%B6)
  - [javadoc - 文档命令帮助](#javadoc---%E6%96%87%E6%A1%A3%E5%91%BD%E4%BB%A4%E5%B8%AE%E5%8A%A9)
  - [**javah命令**](#javah%E5%91%BD%E4%BB%A4)
- [Maven](#maven)
  - [Maven 命令行参数](#maven-%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0)
  - [命名行创建maven项目](#%E5%91%BD%E5%90%8D%E8%A1%8C%E5%88%9B%E5%BB%BAmaven%E9%A1%B9%E7%9B%AE)
- [简介](#%E7%AE%80%E4%BB%8B)
- [基础语法](#%E5%9F%BA%E7%A1%80%E8%AF%AD%E6%B3%95)
- [:point_right:关键字](#point_right%E5%85%B3%E9%94%AE%E5%AD%97)
- [:point_right:类和对象](#point_right%E7%B1%BB%E5%92%8C%E5%AF%B9%E8%B1%A1)
  - [:point_right:变量类型](#point_right%E5%8F%98%E9%87%8F%E7%B1%BB%E5%9E%8B)
  - [:point_right:构造方法](#point_right%E6%9E%84%E9%80%A0%E6%96%B9%E6%B3%95)
  - [:point_right:创建对象](#point_right%E5%88%9B%E5%BB%BA%E5%AF%B9%E8%B1%A1)
  - [:point_right:源文件声明规则](#point_right%E6%BA%90%E6%96%87%E4%BB%B6%E5%A3%B0%E6%98%8E%E8%A7%84%E5%88%99)
  - [:point_right:包](#point_right%E5%8C%85)
  - [:point_right:import](#point_rightimport)
- [:point_right:数据类型](#point_right%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B)
  - [:point_right:**类型默认值**](#point_right%E7%B1%BB%E5%9E%8B%E9%BB%98%E8%AE%A4%E5%80%BC)
  - [:point_right:引用类型](#point_right%E5%BC%95%E7%94%A8%E7%B1%BB%E5%9E%8B)
  - [:point_right:常量](#point_right%E5%B8%B8%E9%87%8F)
  - [:point_right:自动类型转换](#point_right%E8%87%AA%E5%8A%A8%E7%B1%BB%E5%9E%8B%E8%BD%AC%E6%8D%A2)
  - [**:point_right:强制类型转换**](#point_right%E5%BC%BA%E5%88%B6%E7%B1%BB%E5%9E%8B%E8%BD%AC%E6%8D%A2)
- [变量类型](#%E5%8F%98%E9%87%8F%E7%B1%BB%E5%9E%8B)
- [:point_right:Java 修饰符](#point_rightjava-%E4%BF%AE%E9%A5%B0%E7%AC%A6)
  - [:point_right:访问修饰服](#point_right%E8%AE%BF%E9%97%AE%E4%BF%AE%E9%A5%B0%E6%9C%8D)
  - [:point_right:非访问修饰符](#point_right%E9%9D%9E%E8%AE%BF%E9%97%AE%E4%BF%AE%E9%A5%B0%E7%AC%A6)
- [:point_right:Java 运算符](#point_rightjava-%E8%BF%90%E7%AE%97%E7%AC%A6)
- [:point_right:java循环](#point_rightjava%E5%BE%AA%E7%8E%AF)
  - [while](#while)
  - [do…while 循环](#dowhile-%E5%BE%AA%E7%8E%AF)
  - [:point_right:for循环](#point_rightfor%E5%BE%AA%E7%8E%AF)
  - [:point_right:for each 循环](#point_rightfor-each-%E5%BE%AA%E7%8E%AF)
  - [:point_right:break 关键字](#point_rightbreak-%E5%85%B3%E9%94%AE%E5%AD%97)
  - [:point_right:continue 关键字](#point_rightcontinue-%E5%85%B3%E9%94%AE%E5%AD%97)
- [Java 条件执行](#java-%E6%9D%A1%E4%BB%B6%E6%89%A7%E8%A1%8C)
- [:point_right:switch case 语句](#point_rightswitch-case-%E8%AF%AD%E5%8F%A5)
- [:point_right:stringBuffer vs StringBuilder](#point_rightstringbuffer-vs-stringbuilder)
- [:point_right:Java 数组](#point_rightjava-%E6%95%B0%E7%BB%84)
- [Java 方法](#java-%E6%96%B9%E6%B3%95)
  - [可变参数](#%E5%8F%AF%E5%8F%98%E5%8F%82%E6%95%B0)
  - [:point_right:finalize() 方法](#point_rightfinalize-%E6%96%B9%E6%B3%95)
- [Java 异常处理](#java-%E5%BC%82%E5%B8%B8%E5%A4%84%E7%90%86)
  - [:point_right:try](#point_righttry)
  - [**:point_right:throw 关键字**](#point_rightthrow-%E5%85%B3%E9%94%AE%E5%AD%97)
  - [:point_right:**throws 关键字**](#point_rightthrows-%E5%85%B3%E9%94%AE%E5%AD%97)
  - [finally关键字](#finally%E5%85%B3%E9%94%AE%E5%AD%97)
  - [Try-with-resources 语法糖](#try-with-resources-%E8%AF%AD%E6%B3%95%E7%B3%96)
  - [自定义异常](#%E8%87%AA%E5%AE%9A%E4%B9%89%E5%BC%82%E5%B8%B8)
- [:point_right:Java 继承](#point_rightjava-%E7%BB%A7%E6%89%BF)
  - [**:point_right:extends关键字**](#point_rightextends%E5%85%B3%E9%94%AE%E5%AD%97)
  - [**:point_right:implements关键字**](#point_rightimplements%E5%85%B3%E9%94%AE%E5%AD%97)
  - [**:point_right:super 与 this 关键字**](#point_rightsuper-%E4%B8%8E-this-%E5%85%B3%E9%94%AE%E5%AD%97)
  - [**:point_right:final 关键字**](#point_rightfinal-%E5%85%B3%E9%94%AE%E5%AD%97)
  - [构造器](#%E6%9E%84%E9%80%A0%E5%99%A8)
  - [重写(Override)](#%E9%87%8D%E5%86%99override)
  - [重载(Overload)](#%E9%87%8D%E8%BD%BDoverload)
- [Java 多态](#java-%E5%A4%9A%E6%80%81)
  - [多态的实现方式](#%E5%A4%9A%E6%80%81%E7%9A%84%E5%AE%9E%E7%8E%B0%E6%96%B9%E5%BC%8F)
- [:point_right:Java 抽象类](#point_rightjava-%E6%8A%BD%E8%B1%A1%E7%B1%BB)
- [:point_right:Java 封装](#point_rightjava-%E5%B0%81%E8%A3%85)
- [:point_right:Java 接口](#point_rightjava-%E6%8E%A5%E5%8F%A3)
- [:point_right:Java 枚举(enum)](#point_rightjava-%E6%9E%9A%E4%B8%BEenum)
- [:point_right:Java 包(package)](#point_rightjava-%E5%8C%85package)
- [Java Object 类](#java-object-%E7%B1%BB)
- [:point_right:Java 泛型](#point_rightjava-%E6%B3%9B%E5%9E%8B)
- [:point_right:Java 多线程](#point_rightjava-%E5%A4%9A%E7%BA%BF%E7%A8%8B)
  - [通过实现 Runnable 接口来创建线程](#%E9%80%9A%E8%BF%87%E5%AE%9E%E7%8E%B0-runnable-%E6%8E%A5%E5%8F%A3%E6%9D%A5%E5%88%9B%E5%BB%BA%E7%BA%BF%E7%A8%8B)
  - [通过继承Thread来创建线程](#%E9%80%9A%E8%BF%87%E7%BB%A7%E6%89%BFthread%E6%9D%A5%E5%88%9B%E5%BB%BA%E7%BA%BF%E7%A8%8B)
  - [通过 Callable 和 Future 创建线程](#%E9%80%9A%E8%BF%87-callable-%E5%92%8C-future-%E5%88%9B%E5%BB%BA%E7%BA%BF%E7%A8%8B)
- [:point_right:Java 反射 -todo](#point_rightjava-%E5%8F%8D%E5%B0%84--todo)
  - [:point_right:class](#point_rightclass)
  - [:point_right:访问字段](#point_right%E8%AE%BF%E9%97%AE%E5%AD%97%E6%AE%B5)
  - [:point_right:调用方法](#point_right%E8%B0%83%E7%94%A8%E6%96%B9%E6%B3%95)
- [:point_right:注解](#point_right%E6%B3%A8%E8%A7%A3)
  - [:point_right:定义注解](#point_right%E5%AE%9A%E4%B9%89%E6%B3%A8%E8%A7%A3)
  - [:point_right:处理注解](#point_right%E5%A4%84%E7%90%86%E6%B3%A8%E8%A7%A3)
- [Somenote](#somenote)
  - [defualt](#defualt)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

19.03

# :point_right:java环境变量

```Bash
export JAVA_HOME=/Users/bytedance/Java/JavaVirtualMachines/jdk-19.0.2.jdk/Contents/Home
export PATH=$JAVA_HOME/bin:$PATH
```

## :point_right:Java 命令行参数 - 运行java

```Bash
用法：java [options] <主类> [args...]
           （执行类）
   或  java [options] -jar <jar 文件> [args...]
           （执行 jar 文件）
   或  java [options] -m <模块>[/<主类>] [args...]
       java [options] --module <模块>[/<主类>] [args...]
           （执行模块中的主类）
   或  java [options] <源文件> [args]
           （执行单个源文件程序）
```

## :point_right:Javac 命令命令行参数 - 编译java文件

javac是用来将java源代码编译为二进制字节码的编译程序

```Bash
javac <options> <source files>
```

## javadoc - 文档命令帮助

```Bash
-public        仅显示 public 类和成员
-protected        显示 protected/public 类和成员（默认值）
-package        显示 package/protected/public 类和成员
-private        显示所有类和成员
-d <directory>        输出文件的目标目录
-version        包含 @version 段
-author        包含 @author 段
-splitindex        将索引分为每个字母对应一个文件
-windowtitle <text>        文档的浏览器窗口标题
```

@author        标识一个类的作者，一般用于类注释        @author description

@deprecated        指名一个过期的类或成员，表明该类或方法不建议使用        @deprecated description

{@docRoot}        指明当前文档根目录的路径        Directory Path

@exception        可能抛出异常的说明，一般用于方法注释        @exception exception-name explanation

{@inheritDoc}        从直接父类继承的注释        Inherits a comment from the immediate surperclass.

{@link}        插入一个到另一个主题的链接        {@link name text}

{@linkplain}        插入一个到另一个主题的链接，但是该链接显示纯文本字体        Inserts an in-line link to another topic.

@param        说明一个方法的参数，一般用于方法注释        @param parameter-name explanation

@return        说明返回值类型，一般用于方法注释，不能出现再构造方法中        @return explanation

@see        指定一个到另一个主题的链接        @see anchor

@serial        说明一个序列化属性        @serial description

@serialData        说明通过 writeObject() 和 writeExternal() 方法写的数据        @serialData description

@serialField        说明一个 ObjectStreamField 组件        @serialField name type description

@since        说明从哪个版本起开始有了这个函数        @since release

@throws        和 @exception 标签一样.        The @throws tag has the same meaning as the @exception tag.

{@value}        显示常量的值，该常量必须是 static 属性。        Displays the value of a constant, which must be a static field.

@version        指定类的版本，一般用于类注释        @version info

## **javah命令**

javah命令主要用于在JNI开发的时，把java代码声明的JNI方法转化成C\C++[头文件](https://so.csdn.net/so/search?q=头文件&spm=1001.2101.3001.7020)

```Bash
-d 和-o
这两个参数用于设置生成的C\C++头文件的指定，该两参数选项不能同时使用，-d是为中的每个有JNI方法的java类都生成一个头文件，并存放在-d指定的目录中，-o则是生成的所有JNI方法的头文件都放在-o指定的文件中。
-jin
表示用于生成JNI风格的C\C++头文件，默认该参数就是开启的。
-classpath
　使用-classpath后JDK将不再使用CLASSPATH中的类搜索路径，如果-classpath和CLASSPATH都没有设置，则JDK使用当前路径(.)作为类搜索路径。
```

# Maven

```Bash
# Setting PATH for mava 3.9.1
export M3_HOME=/Users/bytedance/Maven/apache-maven-3.9.1
export PATH=$M3_HOME/bin:$PATH
```

## Maven 命令行参数

- mvn -v, –version 显示版本信息;
- mvn -V, –show-version 显示版本信息后继续执行Maven其他目标;
- mvn -h, –help 显示帮助信息; mvn -e, –errors 控制Maven的日志级别,产生执行错误相关消息;
- mvn -X, –debug 控制Maven的日志级别,产生执行调试信息;
- mvn -q, –quiet 控制Maven的日志级别,仅仅显示错误;
- mvn -Pxxx 激活 id 为 xxx的profile (如有多个，用逗号隔开);
- mvn -Dxxx=yyy 指定Java全局属性;
- mvn -o , –offline 运行offline模式,不联网更新依赖;
- mvn -N, –non-recursive 仅在当前项目模块执行命令,不构建子模块;
- mvn -pl, –module_name 在指定模块上执行命令;
- mvn -ff, –fail-fast 遇到构建失败就直接退出;
- mvn -fn, –fail-never 无论项目结果如何,构建从不失败;
- mvn -fae, –fail-at-end 仅影响构建结果,允许不受影响的构建继续;
- mvn -C, –strict-checksums 如果校验码不匹配的话,构建失败;
- mvn -c, –lax-checksums 如果校验码不匹配的话,产生告警;
- mvn -U 强制更新snapshot类型的插件或依赖库(否则maven一天只会更新一次snapshot依赖);
- mvn -npu, –no-plugin-updates 对任何相关的注册插件,不进行最新检查(使用该选项使Maven表现出稳定行为，该稳定行为基于本地仓库当前可用的所有插件版本);
- mvn -cpu, –check-plugin-updates 对任何相关的注册插件,强制进行最新检查(即使项目POM里明确规定了Maven插件版本,还是会强制更新);
- mvn -up, –update-plugins [mvn -cpu]的同义词;
- mvn -B, –batch-mode 在非交互（批处理）模式下运行(该模式下,当Mven需要输入时,它不会停下来接受用户的输入,而是使用合理的默认值);
- mvn -f, –file 强制使用备用的POM文件; mvn -s, –settings 用户配置文件的备用路径;
- mvn -gs, –global-settings 全局配置文件的备用路径;
- mvn -emp, –encrypt-master-password 加密主安全密码,存储到Maven settings文件里;
- mvn -ep, –encrypt-password 加密服务器密码,存储到Maven settings文件里;
- mvn -npr, –no-plugin-registry 对插件版本不使用~/.m2/plugin-registry.xml(插件注册表)里的配置

## 命名行创建maven项目

```Bash
mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

# 简介

Java是 面向对象程序设计语言

解释型语音

# 基础语法

java 程序可以认为是一系列对象的集合

我们可以使用 **-encoding** 选项设置 **utf-8** 来编译

```bash
javac -encoding UTF-8 HelloWorld.java 
java  HelloWorld
```

# :point_right:关键字

- 访问控制
  - private            私有的   当前类可以访问
  - protected        受保护的  同包下可以访问
  - public              公共的 共同访问
  - default             默认   不使用default定义方法的话，该interface的实现类都必须重写所有的抽象方法，但是，在实现含有default方法的接口时
- 类、方法和变量修饰符
  - abstract        声明抽象
  - class        类
  - extends        扩充,继承
  - final        最终值,不可改变的
  - implements        实现（接口）
  - interface        接口
  - native        本地，原生方法（非 Java 实现）
  - new        新,创建
  - static        静态
  - strictfp        严格,精准
  - synchronized        线程,同步
  - transient        短暂
  - volatile        易失
- 程序控制语句
  - break        跳出循环
  - case        定义一个值以供 switch 选择
  - continue        继续
  - do        运行
  - else        否则
  - for        循环
  - if        如果
  - instanceof        实例
  - return        返回
  - switch        根据值选择执行
  - while        循环
- 错误处理
  - assert        断言表达式是否为真
  - catch        捕捉异常
  - finally        有没有异常都执行
  - throw        抛出一个异常对象
  - throws        声明一个异常可能被抛出
  - try        捕获异常
- 包相关        
  - import        引入
  - package        包
- 基本类型        
  - boolean        布尔型
  - byte        字节型
  - char        字符型
  - double        双精度浮点
  - float        单精度浮点
  - int        整型
  - long        长整型
  - short        短整型
- 变量引用        
  - super        父类,超类
  - this        本类
  - void        无返回值
- 保留关键字       
  -  goto        是关键字，但不能使用
  - const        是关键字，但不能使用

> Java 的 null 不是关键字，类似于 true 和 false，它是一个字面常量，不允许作为标识符使用。

# :point_right:类和对象

- 多态
- 继承
- 封装
- 抽象
- 类
- 对象
- 实例
- 方法
- 重载

## :point_right:变量类型

一个类可以包含以下类型变量：

- **局部变量**：在方法、构造方法或者语句块中定义的变量被称为局部变量。变量声明和初始化都是在方法中，方法结束后，变量就会自动销毁。
- **成员变量**：成员变量是定义在类中，方法体之外的变量。这种变量在创建对象的时候实例化。成员变量可以被类中方法、构造方法和特定类的语句块访问。
- **类变量**：类变量也声明在类中，方法体之外，但必须声明为 static 类型。

```Java
public class Dog {
    String breed;
    int size;
    String colour;
    int age;
 
    void eat() {
    }
 
    void run() {
    }
 
    void sleep(){
    }
 
    void name(){
    }
}
```

> 一个类可以拥有多个方法，在上面的例子中：eat()、run()、sleep() 和 name() 都是 Dog 类的方法。

## :point_right:构造方法

构造方法的名称必须与类同名，一个类可以有多个构造方法。 类似于python的__init__

```Java
public class Puppy{
    public Puppy(){
    }
 
    public Puppy(String name){
        // 这个构造器仅有一个参数：name
    }
}
```

## :point_right:创建对象

对象是根据类创建的。在Java中，使用关键字 new 来创建一个新的对象。创建对象需要以下三步：

- **声明**：声明一个对象，包括对象名称和对象类型。
- **实例化**：使用关键字 new 来创建一个对象。
- **初始化**：使用 new 创建对象时，会调用构造方法初始化对象。

```Java
public class Puppy{
   public Puppy(String name){
      //这个构造器仅有一个参数：name
      System.out.println("小狗的名字是 : " + name ); 
   }
   public static void main(String[] args){
      // 下面的语句将创建一个Puppy对象
      Puppy myPuppy = new Puppy( "tommy" );
   }
}
```

## :point_right:源文件声明规则

当在一个源文件中定义多个类，并且还有import语句和package语句时，要特别注意这些规则。

- 一个源文件中只能有一个 public 类
- 一个源文件可以有多个非 public 类
- 源文件的名称应该和 public 类的类名保持一致。例如：源文件中 public 类的类名是 Employee，那么源文件应该命名为Employee.java。
- 如果一个类定义在某个包中，那么 package 语句应该在源文件的首行。
- 如果源文件包含 import 语句，那么应该放在 package 语句和类定义之间。如果没有 package 语句，那么 import 语句应该在源文件中最前面。
- import 语句和 package 语句对源文件中定义的所有类都有效。在同一源文件中，不能给不同的类不同的包声明。

## :point_right:包

包主要用来对类和接口进行分类。

## :point_right:import 

在 Java 中，如果给出一个完整的限定名，包括包名、类名，那么 Java 编译器就可以很容易地定位到源代码或者类

```Java
// 面的命令行将会命令编译器载入 java_installation/java/io 路径下的所有类
import java.io.*;
```

# :point_right:数据类型

java语言提供了八种基本类型。六种数字类型（四个整数型，两个浮点型），一种字符类型，还有一种布尔型。

- byte    对应golang int8
- short  对应golang int16
- int       对应golang int32
- long    对应golang int64 
- float    对应golang float32 
- double  对应 golang float64
- **boolean 对应 bool**
- **char    对应unicode编码** **golang** **uint32**

## :point_right:**类型默认值**

| **数据类型**           | **默认值** |
| ---------------------- | ---------- |
| byte                   | 0          |
| short                  | 0          |
| int                    | 0          |
| long                   | 0L         |
| float                  | 0.0f       |
| double                 | 0.0d       |
| char                   | 'u0000'    |
| String (or any object) | null       |
| boolean                | false      |

## :point_right:引用类型

在Java中，引用类型的变量非常类似于C/C++的指针。引用类型指向一个对象，指向对象的变量是引用变量。

变量一旦声明后，类型就不能被改变了。

- 对象、数组都是引用数据类型。
- 所有引用类型的默认值都是null。
- 一个引用变量可以用来引用任何与之兼容的类型。
- 例子：Site site = new Site("Runoob")。

## :point_right:常量

在 Java 中使用 final 关键字来修饰常量，声明方式和变量类似：

```Bash
final double PI = 3.1415927;
```

## :point_right:自动类型转换

低 - >  高

byte,short,char—> int —> long—> float —> double

```Java
 // 转换时需要判断精度丢失问题
int i =128;   
byte b = (byte)i;
```

## **:point_right:强制类型转换**

1. 条件是转换的数据类型必须是兼容的。
2. 格式：(type)value type是要强制类型转换后的数据类型 实例：

```Java
public class QiangZhiZhuanHuan{
    public static void main(String[] args){
        int i1 = 123;
        byte b = (byte)i1;//强制类型转换为byte
        System.out.println("int强制类型转换为byte后的值等于"+b);
    }
}
```

# 变量类型

Java语言支持的变量类型有：

- 类变量：独立于方法之外的变量，用 static 修饰。
- 实例变量：独立于方法之外的变量，不过没有 static 修饰。
- 局部变量：类的方法中的变量。

类变量（静态变量）

- 类变量也称为静态变量，在类中以 static 关键字声明，但必须在方法之外。
- 无论一个类创建了多少个对象，类只拥有类变量的一份拷贝。
- 静态变量除了被声明为常量外很少使用，静态变量是指声明为 public/private，final 和 static 类型的变量。静态变量初始化后不可改变。
- 静态变量储存在静态存储区。经常被声明为常量，很少单独使用 static 声明变量。
- 静态变量在第一次被访问时创建，在程序结束时销毁。
- 与实例变量具有相似的可见性。但为了对类的使用者可见，大多数静态变量声明为 public 类型。
- 默认值和实例变量相似。数值型变量默认值是 0，布尔型默认值是 false，引用类型默认值是 null。变量的值可以在声明的时候指定，也可以在构造方法中指定。此外，静态变量还可以在静态语句块中初始化。
- 静态变量可以通过：*ClassName.VariableName*的方式访问。
- 类变量被声明为 public static final 类型时，类变量名称一般建议使用大写字母。如果静态变量不是 public 和 final 类型，其命名方式与实例变量以及局部变量的命名方式一致。

# :point_right:Java 修饰符

Java语言提供了很多修饰符，主要分为以下两类：

- 访问修饰符
- 非访问修饰符

## :point_right:访问修饰服

Java中，可以使用访问控制符来保护对类、变量、方法和构造方法的访问。Java 支持 4 种不同的访问权限。

- **default** (即默认，什么也不写）: 在同一包内可见，不使用任何修饰符。使用对象：类、接口、变量、方法。
- **private** : 在同一类内可见。使用对象：变量、方法。 **注意：不能修饰类（外部类）**
- **public** : 对所有类可见。使用对象：类、接口、变量、方法
- **protected** : 对同一包内的类和所有子类可见。使用对象：变量、方法。 **注意：不能修饰类（外部类）**。

**访问控制和继承**

请注意以下方法继承的规则：

- 父类中声明为 public 的方法在子类中也必须为 public。
- 父类中声明为 protected 的方法在子类中要么声明为 protected，要么声明为 public，不能声明为 private。
- 父类中声明为 private 的方法，不能够被子类继承。

## :point_right:非访问修饰符

为了实现一些其他的功能，Java 也提供了许多非访问修饰符。

static 修饰符，用来修饰类方法和类变量。

final 修饰符，用来修饰类、方法和变量，final 修饰的类不能够被继承，修饰的方法不能被继承类重新定义，修饰的变量为常量，是不可修改的。

abstract 修饰符，用来创建抽象类和抽象方法。

抽象类不能用来实例化对象，声明抽象类的唯一目的是为了将来对该类进行扩充。

```Java
abstract class Caravan{
   private double price;
   private String model;
   private String year;
   public abstract void goFast(); //抽象方法
   public abstract void changeColor();
}
```

抽象方法

抽象方法是一种没有任何实现的方法，该方法的具体实现由子类提供。

抽象方法不能被声明成 final 和 static。

```Java
public abstract class SuperClass{
    abstract void m(); //抽象方法
}
 
class SubClass extends SuperClass{
     //实现抽象方法
      void m(){
          .........
      }
}
```

synchronized 和 volatile 修饰符，主要用于线程的编程。

synchronized 关键字声明的方法同一时间只能被一个线程访问。synchronized 修饰符可以应用于四个访问修饰符。

```Java
public synchronized void showDetails(){
.......
}
```

**transient 修饰符 ：** 

序列化的对象包含被 transient 修饰的实例变量时，java 虚拟机(JVM)跳过该特定的变量。

该修饰符包含在定义变量的语句中，用来预处理类和变量的数据类型。

```Java
public transient int limit = 55;   // 不会持久化
public int b; // 持久化
```

**volatile 修饰符**

volatile 修饰的成员变量在每次被线程访问时，都强制从共享内存中重新读取该成员变量的值。而且，当成员变量发生变化时，会强制线程将变化值回写到共享内存。这样在任何时刻，两个不同的线程总是看到某个成员变量的同一个值。

一个 volatile 对象引用可能是 null。

```Java
public class MyRunnable implements Runnable
{
    private volatile boolean active;
    public void run()
    {
        active = true;
        while (active) // 第一行
        {
            // 代码
        }
    }
    public void stop()
    {
        active = false; // 第二行
    }
}
```

# :point_right:Java 运算符 

和其他类似

# :point_right:java循环

Java中有三种主要的循环结构：

- **while** 循环
- **do…while** 循环
- **for** 循环

## while

只要布尔表达式为 true，循环就会一直执行下去。

```Java
int x = 10;
while( x < 20 ) {
     System.out.print("value of x : " + x );
     x++;
     System.out.print("\n");
}
```

## do…while 循环

对于 while 语句而言，如果不满足条件，则不能进入循环。但有时候我们需要即使不满足条件，也至少执行一次。

do…while 循环和 while 循环相似，不同的是，do…while 循环至少会执行一次。

```Java
int x = 10;
do{
     System.out.print("value of x : " + x );
     x++;
     System.out.print("\n");
}while( x < 20 );
```

## :point_right:for循环

for循环执行的次数是在执行前就确定的。语法格式如下：

```Java
for(初始化; 布尔表达式; 更新) {
    //代码语句
}

for(int x = 10; x < 20; x = x+1) {
         System.out.print("value of x : " + x );
         System.out.print("\n");
      }
```

## :point_right:for each 循环

```Java
for(声明语句 : 表达式)
{
   //代码句子
}

String [] names ={"James", "Larry", "Tom", "Lacy"};
for( String name : names ) {
     System.out.print( name );
     System.out.print(",");
}
```

## :point_right:break 关键字

break 主要用在循环语句或者 switch 语句中，用来跳出整个语句块。

break 跳出最里层的循环，并且继续执行该循环下面的语句。

可以指定flag，break flag 跳出指定循环

## :point_right:continue 关键字

continue 适用于任何循环控制结构中。作用是让程序立刻跳转到下一次循环的迭代。

在 for 循环中，continue 语句使程序立即跳转到更新语句。

在 while 或者 do…while 循环中，程序立即跳转到布尔表达式的判断语句。

# Java 条件执行

```Java
if(布尔表达式)
{
   //如果布尔表达式为true将执行的语句
}

// if else
if(布尔表达式){
   //如果布尔表达式的值为true
}else{
   //如果布尔表达式的值为false
}

// if...else if...else
if(布尔表达式 1){
   //如果布尔表达式 1的值为true执行代码
}else if(布尔表达式 2){
   //如果布尔表达式 2的值为true执行代码
}else if(布尔表达式 3){
   //如果布尔表达式 3的值为true执行代码
}else {
   //如果以上布尔表达式都不为true执行代码
}

// 嵌套if
if(布尔表达式 1){
   ////如果布尔表达式 1的值为true执行代码
   if(布尔表达式 2){
      ////如果布尔表达式 2的值为true执行代码
   }
}
```

# :point_right:switch case 语句

```Java
switch(expression){
    case value :
       //语句
       break; //可选
    case value :
       //语句
       break; //可选
    //你可以有任意数量的case语句
    default : //可选
       //语句
}
```

**witch case 执行时，一定会先进行匹配，匹配成功返回当前 case 的值，再根据是否有 break，判断是否继续输出，或是跳出判断。**

# :point_right:stringBuffer vs StringBuilder

它和 StringBuffer 之间的最大不同在于 StringBuilder 的方法不是线程安全的（不能同步访问）。

由于 StringBuilder 相较于 StringBuffer 有速度优势，所以多数情况下建议使用 StringBuilder 类。

# :point_right:Java 数组

```Java
dataType[] arrayRefVar;   // 首选的方法
// 或
dataType arrayRefVar[];  // 效果相同，但不是首选方法

double[] myList = new double[size];
// 打印所有数组元素
for (int i = 0; i < myList.length; i++) {
     System.out.println(myList[i] + " ");
}
for (double element: myList) {
     System.out.println(element);
}


// 多维
String[][] str = new String[3][4];
```

# Java 方法

## 可变参数

一个方法中只能指定一个可变参数，它必须是方法的最后一个参数。任何普通的参数必须在它之前声明。和golang 类似。

typeName... parameterName

```Bash
public static void printMax( double... numbers) {
        if (numbers.length == 0) {
            System.out.println("No argument passed");
            return;
        }
 
        double result = numbers[0];
 
        for (int i = 1; i <  numbers.length; i++){
            if (numbers[i] >  result) {
                result = numbers[i];
            }
        }
        System.out.println("The max value is " + result);
    }
```

## :point_right:finalize() 方法

Java 允许定义这样的方法，它在对象被垃圾收集器析构(回收)之前调用，这个方法叫做 finalize( )，它用来清除回收对象。

```Java
class Cake extends Object {  
  private int id;  
  public Cake(int id) {  
    this.id = id;  
    System.out.println("Cake Object " + id + "is created");  
  }  
    
  protected void finalize() throws java.lang.Throwable {  
    super.finalize();  
    System.out.println("Cake Object " + id + "is disposed");  
  }  
}
```

# Java 异常处理

## :point_right:try

```Java
try{
   // 程序代码
}catch(异常类型1 异常的变量名1){
  // 程序代码
}catch(异常类型2 异常的变量名2){
  // 程序代码
}catch(异常类型3 异常的变量名3){
  // 程序代码
}
```

## **:point_right:throw 关键字**

**throw** 关键字用于在当前方法中抛出一个异常。

```Java
public void checkNumber(int num) {
  if (num < 0) {
    throw new IllegalArgumentException("Number must be positive");
  }
}
```

## :point_right:**throws 关键字**

**throws** 关键字用于在方法声明中指定该方法可能抛出的异常。当方法内部抛出指定类型的异常时，该异常会被传递给调用该方法的代码，并在该代码中处理异常。

例如，下面的代码中，当 readFile 方法内部发生 IOException 异常时，会将该异常传递给调用该方法的代码。在调用该方法的代码中，必须捕获或声明处理 IOException 异常。

```Java
public void readFile(String filePath) throws IOException {
      BufferedReader reader = new BufferedReader(new FileReader(filePath));
      String line = reader.readLine();
      while (line != null) {
        System.out.println(line);
        line = reader.readLine();
      }
      reader.close();
}
```

## finally关键字

finally 关键字用来创建在 try 代码块后面执行的代码块。

无论是否发生异常，finally 代码块中的代码总会被执行。

```Java
try{
  // 程序代码
}catch(异常类型1 异常的变量名1){
  // 程序代码
}catch(异常类型2 异常的变量名2){
  // 程序代码
}finally{
  // 程序代码
}
```

## Try-with-resources 语法糖

Java 新增的 **try-with-resource** 语法糖来打开资源，并且可以在语句执行完毕后确保每个资源都被自动关闭 。

```Java
try (resource declaration) {
  // 使用的资源
} catch (ExceptionType e1) {
  // 异常块
}

// 例子
import java.io.*;

public class RunoobTest {

    public static void main(String[] args) {
    String line;
        try(BufferedReader br = new BufferedReader(new FileReader("test.txt"))) {
            while ((line = br.readLine()) != null) {
                System.out.println("Line =>"+line);
            }
        } catch (IOException e) {
            System.out.println("IOException in try block =>" + e.getMessage());
        }
    }
}
```

## 自定义异常

在 Java 中你可以自定义异常。编写自己的异常类时需要记住下面的几点。

- 所有异常都必须是 Throwable 的子类。
- 如果希望写一个检查性异常类，则需要继承 Exception 类。
- 如果你想写一个运行时异常类，那么需要继承 RuntimeException 类。

```Java
import java.io.*;
 
//自定义异常类，继承Exception类
public class InsufficientFundsException extends Exception
{
  //此处的amount用来储存当出现异常（取出钱多于余额时）所缺乏的钱
  private double amount;
  public InsufficientFundsException(double amount)
  {
    this.amount = amount;
  } 
  public double getAmount()
  {
    return amount;
  }
}


// 文件名称 CheckingAccount.java
import java.io.*;
 
//此类模拟银行账户
public class CheckingAccount
{
  //balance为余额，number为卡号
   private double balance;
   private int number;
   public CheckingAccount(int number)
   {
      this.number = number;
   }
  //方法：存钱
   public void deposit(double amount)
   {
      balance += amount;
   }
  //方法：取钱
   public void withdraw(double amount) throws
                              InsufficientFundsException
   {
      if(amount <= balance)
      {
         balance -= amount;
      }
      else
      {
         double needs = amount - balance;
         throw new InsufficientFundsException(needs);
      }
   }
  //方法：返回余额
   public double getBalance()
   {
      return balance;
   }
  //方法：返回卡号
   public int getNumber()
   {
      return number;
   }
}
```

# :point_right:Java 继承

## **:point_right:extends关键字**

在 Java 中通过 extends 关键字可以申明一个类是从另外一个类继承而来的，一般形式如下：

类的继承是单一继承，也就是说，一个子类只能拥有一个父类，所以 extends 只能继承一个类。

```Java
class 父类 {
}
 
class 子类 extends 父类 {
}
```

## **:point_right:implements关键字**

使用 implements 关键字可以变相的使java具有多继承的特性，使用范围为类继承接口的情况，可以同时继承多个接口（接口跟接口之间采用逗号分隔）。

```Java
public interface A {
    public void eat();
    public void sleep();
}
 
public interface B {
    public void show();
}
 
public class C implements A,B {
}
```

## **:point_right:super 与 this 关键字**

super关键字：我们可以通过super关键字来实现对父类成员的访问，用来引用当前对象的父类。

this关键字：指向自己的引用。

```Java
class Animal {
  void eat() {
    System.out.println("animal : eat");
  }
}
 
class Dog extends Animal {
  void eat() {
    System.out.println("dog : eat");
  }
  void eatTest() {
    this.eat();   // this 调用自己的方法
    super.eat();  // super 调用父类方法
  }
}
 
public class Test {
  public static void main(String[] args) {
    Animal a = new Animal();
    a.eat();
    Dog d = new Dog();
    d.eatTest();
  }
}
```

## **:point_right:final 关键字**

final 可以用来修饰变量（包括类属性、对象属性、局部变量和形参）、方法（包括类方法和对象方法）和类。

final 含义为 "最终的"。

使用 final 关键字声明类，就是把类定义定义为最终类，不能被继承，或者用于修饰方法，该方法不能被子类重写：

> final 定义的类，其中的属性、方法不是 final 的。

## 构造器

子类是不继承父类的构造器（构造方法或者构造函数）的，它只是调用（隐式或显式）。如果父类的构造器带有参数，则必须在子类的构造器中显式地通过 **super** 关键字调用父类的构造器并配以适当的参数列表。

```Java
class SuperClass {
  private int n;
  SuperClass(){
    System.out.println("SuperClass()");
  }
  SuperClass(int n) {
    System.out.println("SuperClass(int n)");
    this.n = n;
  }
}
// SubClass 类继承
class SubClass extends SuperClass{
  private int n;
  
  SubClass(){ // 自动调用父类的无参数构造器
    System.out.println("SubClass");
  }  
  
  public SubClass(int n){ 
    super(300);  // 调用父类中带有参数的构造器
    System.out.println("SubClass(int n):"+n);
    this.n = n;
  }
}
// SubClass2 类继承
class SubClass2 extends SuperClass{
  private int n;
  
  SubClass2(){
    super(300);  // 调用父类中带有参数的构造器
    System.out.println("SubClass2");
  }  
  
  public SubClass2(int n){ // 自动调用父类的无参数构造器
    System.out.println("SubClass2(int n):"+n);
    this.n = n;
  }
}
public class TestSuperSub{
  public static void main (String args[]){
    System.out.println("------SubClass 类继承------");
    SubClass sc1 = new SubClass();
    SubClass sc2 = new SubClass(100); 
    System.out.println("------SubClass2 类继承------");
    SubClass2 sc3 = new SubClass2();
    SubClass2 sc4 = new SubClass2(200); 
  }
}
```

## 重写(Override)

重写是子类对父类的允许访问的方法的实现过程进行重新编写, 返回值和形参都不能改变。**即外壳不变，核心重写！**

重写的好处在于子类可以根据需要，定义特定于自己的行为。 也就是说子类能够根据需要实现父类的方法。

重写方法不能抛出新的检查异常或者比被重写方法申明更加宽泛的异常。

```Java
class Animal{
   public void move(){
      System.out.println("动物可以移动");
   }
}
 
class Dog extends Animal{
   public void move(){
      System.out.println("狗可以跑和走");
      // 当需要在子类中调用父类的被重写方法时，要使用 super 关键字。
      super.move(); // 应用super类的方法
   }
}
 
public class TestDog{
   public static void main(String args[]){
      Animal a = new Animal(); // Animal 对象
      Animal b = new Dog(); // Dog 对象
 
      a.move();// 执行 Animal 类的方法
 
      b.move();//执行 Dog 类的方法
   }
}
```

## 重载(Overload)

重载(overloading) 是在一个类里面，方法名字相同，而参数不同。返回类型可以相同也可以不同。

每个重载的方法（或者构造函数）都必须有一个独一无二的参数类型列表。

最常用的地方就是构造器的重载。

```Java
public class Overloading {
    public int test(){
        System.out.println("test1");
        return 1;
    }
 
    public void test(int a){
        System.out.println("test2");
    }   
 
    //以下两个参数类型顺序不同
    public String test(int a,String s){
        System.out.println("test3");
        return "returntest3";
    }   
 
    public String test(String s,int a){
        System.out.println("test4");
        return "returntest4";
    }   
 
    public static void main(String[] args){
        Overloading o = new Overloading();
        System.out.println(o.test());
        o.test(1);
        System.out.println(o.test(1,"test3"));
        System.out.println(o.test("test4",1));
    }
}
```

# Java 多态

多态是同一个行为具有多个不同表现形式或形态的能力。

多态就是同一个接口，使用不同的实例而执行不同操作

```Java
public class Test {
    public static void main(String[] args) {
      show(new Cat());  // 以 Cat 对象调用 show 方法
      show(new Dog());  // 以 Dog 对象调用 show 方法
                
      Animal a = new Cat();  // 向上转型  
      a.eat();               // 调用的是 Cat 的 eat
      Cat c = (Cat)a;        // 向下转型  
      c.work();        // 调用的是 Cat 的 work
  }  
            
    public static void show(Animal a)  {
      a.eat();  
        // 类型判断
        if (a instanceof Cat)  {  // 猫做的事情 
            Cat c = (Cat)a;  
            c.work();  
        } else if (a instanceof Dog) { // 狗做的事情 
            Dog c = (Dog)a;  
            c.work();  
        }  
    }  
}
 
abstract class Animal {  
    abstract void eat();  
}  
  
class Cat extends Animal {  
    public void eat() {  
        System.out.println("吃鱼");  
    }  
    public void work() {  
        System.out.println("抓老鼠");  
    }  
}  
  
class Dog extends Animal {  
    public void eat() {  
        System.out.println("吃骨头");  
    }  
    public void work() {  
        System.out.println("看家");  
    }  
}
```

## 多态的实现方式

- **重写**
- **接口**
- **抽象类和抽象方法**

# :point_right:Java 抽象类

在面向对象的概念中，所有的对象都是通过类来描绘的，但是反过来，并不是所有的类都是用来描绘对象的，如果一个类中没有包含足够的信息来描绘一个具体的对象，这样的类就是抽象类。

```Java
/* 文件名 : Employee.java */
public abstract class Employee
{
   private String name;
   private String address;
   private int number;
   public Employee(String name, String address, int number)
   {
      System.out.println("Constructing an Employee");
      this.name = name;
      this.address = address;
      this.number = number;
   }
   public double computePay()
   {
     System.out.println("Inside Employee computePay");
     return 0.0;
   }
   public void mailCheck()
   {
      System.out.println("Mailing a check to " + this.name
       + " " + this.address);
   }
   public String toString()
   {
      return name + " " + address + " " + number;
   }
   public String getName()
   {
      return name;
   }
   public String getAddress()
   {
      return address;
   }
   public void setAddress(String newAddress)
   {
      address = newAddress;
   }
   public int getNumber()
   {
     return number;
   }
}
```

抽象类总结：

1. 抽象类不能被实例化(初学者很容易犯的错)，如果被实例化，就会报错，编译无法通过。只有抽象类的非抽象子类可以创建对象。
2. 抽象类中不一定包含抽象方法，但是有抽象方法的类必定是抽象类。
3. 抽象类中的抽象方法只是声明，不包含方法体，就是不给出方法的具体实现也就是方法的具体功能。
4. 构造方法，类方法（用 static 修饰的方法）不能声明为抽象方法。
5. 抽象类的子类必须给出抽象类中的抽象方法的具体实现，除非该子类也是抽象类。

# :point_right:Java 封装

**封装的优点**

1. 良好的封装能够减少耦合。
2. 类内部的结构可以自由修改。
3. 可以对成员变量进行更精确的控制。
4. 隐藏信息，实现细节。

```Java
/* 文件名: EncapTest.java */
public class EncapTest{
 
   private String name;
   private String idNum;
   private int age;
 
   public int getAge(){
      return age;
   }
 
   public String getName(){
      return name;
   }
 
   public String getIdNum(){
      return idNum;
   }
 
   public void setAge( int newAge){
      age = newAge;
   }
 
   public void setName(String newName){
      name = newName;
   }
 
   public void setIdNum( String newId){
      idNum = newId;
   }
}
```

# :point_right:Java 接口

**接口与类相似点：**

- 一个接口可以有多个方法。
- 接口文件保存在 .java 结尾的文件中，文件名使用接口名。
- 接口的字节码文件保存在 .class 结尾的文件中。
- 接口相应的字节码文件必须在与包名称相匹配的目录结构中。

**接口与类的区别：**

- 接口不能用于实例化对象。
- 接口没有构造方法。
- 接口中所有的方法必须是抽象方法，Java 8 之后 接口中可以使用 default 关键字修饰的非抽象方法。
- 接口不能包含成员变量，除了 static 和 final 变量。
- 接口不是被类继承了，而是要被类实现。
- 接口支持多继承。

**接口特性**

- 接口中每一个方法也是隐式抽象的,接口中的方法会被隐式的指定为 **public abstract**（只能是 public abstract，其他修饰符都会报错）。
- 接口中可以含有变量，但是接口中的变量会被隐式的指定为 **public static final** 变量（并且只能是 public，用 private 修饰会报编译错误）。
- 接口中的方法是不能在接口中实现的，只能由实现接口的类来实现接口中的方法。

**抽象类和接口的区别**

1. 抽象类中的方法可以有方法体，就是能实现方法的具体功能，但是接口中的方法不行。
2. 抽象类中的成员变量可以是各种类型的，而接口中的成员变量只能是 **public static final** 类型的。
3. 接口中不能含有静态代码块以及静态方法(用 static 修饰的方法)，而抽象类是可以有静态代码块和静态方法。
4. 一个类只能继承一个抽象类，而一个类却可以实现多个接口。

```Java
[可见度] interface 接口名称 [extends 其他的接口名] {
        // 声明变量
        // 抽象方法
}
```

接口有以下特性：

- 接口是隐式抽象的，当声明一个接口的时候，不必使用**abstract**关键字。
- 接口中每一个方法也是隐式抽象的，声明时同样不需要**abstract**关键字。
- 接口中的方法都是公有的。

```Java
/* 文件名 : Animal.java */
interface Animal {
   public void eat();
   public void travel();
}
```

# :point_right:Java 枚举(enum)

Java 枚举是一个特殊的类，一般表示一组常量，比如一年的 4 个季节，一个年的 12 个月份，一个星期的 7 天，方向有东南西北等。

```Java
enum Color
{
    RED, GREEN, BLUE;
}
 
public class Test
{
    // 执行输出结果
    public static void main(String[] args)
    {
        Color c1 = Color.RED;
        System.out.println(c1);
    }
}
```

# :point_right:Java 包(package)

为了更好地组织类，Java 提供了包机制，用于区别类名的命名空间。

**包的作用**

- 1、把功能相似或相关的类或接口组织在同一个包中，方便类的查找和使用。
- 2、如同文件夹一样，包也采用了树形目录的存储方式。同一个包中的类名字是不同的，不同的包中的类的名字是可以相同的，当同时调用两个不同包中相同类名的类时，应该加上包名加以区别。因此，包可以避免名字冲突。
- 3、包也限定了访问权限，拥有包访问权限的类才能访问某个包中的类。

类目录的绝对路径叫做 **class path**。设置在系统变量 **CLASSPATH** 中。编译器和 java 虚拟机通过将 package 名字加到 class path 后来构造 .class 文件的路径。

<path- two>\classes 是 class path，package 名字是 com.runoob.test,而编译器和 JVM 会在 <path-two>\classes\com\runoob\test 中找 .class 文件。

一个 class path 可能会包含好几个路径，多路径应该用分隔符分开。默认情况下，编译器和 JVM 查找当前目录。JAR 文件按包含 Java 平台相关的类，所以他们的目录默认放在了 class path 中。

# Java Object 类

Java Object 类是所有类的父类，也就是说 Java 的所有类都继承了 Object，**子类可以使用 Object 的所有方法**。

显式继承:

```Java
public class Runoob extends Object{

}
```

隐式继承:

```Java
public class Runoob {

}
```

类方法

1        protected Object clone()

创建并返回一个对象的拷贝

2        boolean equals(Object obj)

比较两个对象是否相等

3        protected void finalize()

当 GC (垃圾回收器)确定不存在对该对象的有更多引用时，由对象的垃圾回收器调用此方法。

4        Class<?> getClass()

获取对象的运行时对象的类

5        int hashCode()

获取对象的 hash 值

6        void notify()

唤醒在该对象上等待的某个线程

7        void notifyAll()

唤醒在该对象上等待的所有线程

8        String toString()

返回对象的字符串表示形式

9        void wait()

让当前线程进入等待状态。直到其他线程调用此对象的 notify() 方法或 notifyAll() 方法。

10        void wait(long timeout)

让当前线程处于等待(阻塞)状态，直到其他线程调用此对象的 notify() 方法或 notifyAll() 方法，或者超过参数设置的timeout超时时间。

11        void wait(long timeout, int nanos)

与 wait(long timeout) 方法类似，多了一个 nanos 参数，这个参数表示额外时间（以纳秒为单位，范围是 0-999999）。 所以超时的时间还需要加上 nanos 纳秒。。

# :point_right:Java 泛型

你可以写一个泛型方法，该方法在调用时可以接收不同类型的参数。根据传递给泛型方法的参数类型，编译器适当地处理每一个方法调用。

下面是定义泛型方法的规则：

- 所有泛型方法声明都有一个类型参数声明部分（由尖括号分隔），该类型参数声明部分在方法返回类型之前（在下面例子中的 **<E>**）。
- 每一个类型参数声明部分包含一个或多个类型参数，参数间用逗号隔开。一个泛型参数，也被称为一个类型变量，是用于指定一个泛型类型名称的标识符。
- 类型参数能被用来声明返回值类型，并且能作为泛型方法得到的实际参数类型的占位符。
- 泛型方法体的声明和其他方法一样。注意类型参数只能代表引用型类型，不能是原始类型（像 **int、double、char** 等）。

**java** **中泛型标记符：**

- **E** - Element (在集合中使用，因为集合中存放的是元素)
- **T** - Type（Java 类）
- **K** - Key（键）
- **V** - Value（值）
- **N** - Number（数值类型）
- **？** - 表示不确定的 java 类型

```Java
public class GenericMethodTest
{
   // 泛型方法 printArray                         
   public static < E > void printArray( E[] inputArray )
   {
      // 输出数组元素            
         for ( E element : inputArray ){        
            System.out.printf( "%s ", element );
         }
         System.out.println();
    }
 
    public static void main( String args[] )
    {
        // 创建不同类型数组： Integer, Double 和 Character
        Integer[] intArray = { 1, 2, 3, 4, 5 };
        Double[] doubleArray = { 1.1, 2.2, 3.3, 4.4 };
        Character[] charArray = { 'H', 'E', 'L', 'L', 'O' };
 
        System.out.println( "整型数组元素为:" );
        printArray( intArray  ); // 传递一个整型数组
 
        System.out.println( "\n双精度型数组元素为:" );
        printArray( doubleArray ); // 传递一个双精度型数组
 
        System.out.println( "\n字符型数组元素为:" );
        printArray( charArray ); // 传递一个字符型数组
    } 
}
```

# :point_right:Java 多线程

Java 提供了三种创建线程的方法：

- 通过实现 Runnable 接口；
- 通过继承 Thread 类本身；
- 通过 Callable 和 Future 创建线程。

## 通过实现 Runnable 接口来创建线程

创建一个线程，最简单的方法是创建一个实现 Runnable 接口的类。

为了实现 Runnable，一个类只需要执行一个方法调用 run()，

这里，threadOb 是一个实现 Runnable 接口的类的实例，并且 threadName 指定新线程的名字。

新线程创建之后，你调用它的 start() 方法它才会运行。

声明如下：

```Java
class RunnableDemo implements Runnable {
   private Thread t;
   private String threadName;
   
   RunnableDemo( String name) {
      threadName = name;
      System.out.println("Creating " +  threadName );
   }
   
   public void run() {
      System.out.println("Running " +  threadName );
      try {
         for(int i = 4; i > 0; i--) {
            System.out.println("Thread: " + threadName + ", " + i);
            // 让线程睡眠一会
            Thread.sleep(50);
         }
      }catch (InterruptedException e) {
         System.out.println("Thread " +  threadName + " interrupted.");
      }
      System.out.println("Thread " +  threadName + " exiting.");
   }
   
   public void start () {
      System.out.println("Starting " +  threadName );
      if (t == null) {
         t = new Thread (this, threadName);
         t.start ();
      }
   }
}
 
public class TestThread {
   public static void main(String args[]) {
      RunnableDemo R1 = new RunnableDemo( "Thread-1");
      R1.start();
      
      RunnableDemo R2 = new RunnableDemo( "Thread-2");
      R2.start();
   }   
}
```

## 通过继承Thread来创建线程

创建一个线程的第二种方法是创建一个新的类，该类继承 Thread 类，然后创建一个该类的实例。

继承类必须重写 run() 方法，该方法是新线程的入口点。它也必须调用 start() 方法才能执行。

该方法尽管被列为一种多线程实现方式，但是本质上也是实现了 Runnable 接口的一个实例。

```Java
class ThreadDemo extends Thread {
   private Thread t;
   private String threadName;
   
   ThreadDemo( String name) {
      threadName = name;
      System.out.println("Creating " +  threadName );
   }
   
   public void run() {
      System.out.println("Running " +  threadName );
      try {
         for(int i = 4; i > 0; i--) {
            System.out.println("Thread: " + threadName + ", " + i);
            // 让线程睡眠一会
            Thread.sleep(50);
         }
      }catch (InterruptedException e) {
         System.out.println("Thread " +  threadName + " interrupted.");
      }
      System.out.println("Thread " +  threadName + " exiting.");
   }
   
   public void start () {
      System.out.println("Starting " +  threadName );
      if (t == null) {
         t = new Thread (this, threadName);
         t.start ();
      }
   }
}
 
public class TestThread {
 
   public static void main(String args[]) {
      ThreadDemo T1 = new ThreadDemo( "Thread-1");
      T1.start();
      
      ThreadDemo T2 = new ThreadDemo( "Thread-2");
      T2.start();
   }   
}
```

## 通过 Callable 和 Future 创建线程

1. 创建 Callable 接口的实现类，并实现 call() 方法，该 call() 方法将作为线程执行体，并且有返回值。
2. 创建 Callable 实现类的实例，使用 FutureTask 类来包装 Callable 对象，该 FutureTask 对象封装了该 Callable 对象的 call() 方法的返回值。
3. 使用 FutureTask 对象作为 Thread 对象的 target 创建并启动新线程。
4. 调用 FutureTask 对象的 get() 方法来获得子线程执行结束后的返回值

```Java
public class CallableThreadTest implements Callable<Integer> {
    public static void main(String[] args)  
    {  
        CallableThreadTest ctt = new CallableThreadTest();  
        FutureTask<Integer> ft = new FutureTask<>(ctt);  
        for(int i = 0;i < 100;i++)  
        {  
            System.out.println(Thread.currentThread().getName()+" 的循环变量i的值"+i);  
            if(i==20)  
            {  
                new Thread(ft,"有返回值的线程").start();  
            }  
        }  
        try  
        {  
            System.out.println("子线程的返回值："+ft.get());  
        } catch (InterruptedException e)  
        {  
            e.printStackTrace();  
        } catch (ExecutionException e)  
        {  
            e.printStackTrace();  
        }  
  
    }
    @Override  
    public Integer call() throws Exception  
    {  
        int i = 0;  
        for(;i<100;i++)  
        {  
            System.out.println(Thread.currentThread().getName()+" "+i);  
        }  
        return i;  
    }  
}
```

1. 采用实现 Runnable、Callable 接口的方式创建多线程时，线程类只是实现了 Runnable 接口或 Callable 接口，还可以继承其他类。
2. 使用继承 Thread 类的方式创建多线程时，编写简单，如果需要访问当前线程，则无需使用 Thread.currentThread() 方法，直接使用 this 即可获得当前线程。

# :point_right:Java 反射 -todo

反射就是Reflection，Java的反射是指程序在运行期可以拿到一个对象的所有信息。

## :point_right:class

除了int等基本类型外，Java的其他类型全部都是class（包括interface）。例如：

如何获取一个`class`的`Class`实例？有三个方法：

方法一：直接通过一个`class`的静态变量`class`获取：

```Plaintext
Class cls = String.class;
```

方法二：如果我们有一个实例变量，可以通过该实例变量提供的`getClass()`方法获取：

```Plaintext
String s = "Hello";
Class cls = s.getClass();
```

方法三：如果知道一个`class`的完整类名，可以通过静态方法`Class.forName()`获取：

```Plaintext
Class cls = Class.forName("java.lang.String");
```

## :point_right:访问字段

`Class`类提供了以下几个方法来获取字段：

- Field getField(name)：根据字段名获取某个public的field（包括父类）
- Field getDeclaredField(name)：根据字段名获取当前类的某个field（不包括父类）
- Field[] getFields()：获取所有public的field（包括父类）
- Field[] getDeclaredFields()：获取当前类的所有field（不包括父类）

```Java
public class Main {
    public static void main(String[] args) throws Exception {
        Class stdClass = Student.class;
        // 获取public字段"score":
        System.out.println(stdClass.getField("score"));
        // 获取继承的public字段"name":
        System.out.println(stdClass.getField("name"));
        // 获取private字段"grade":
        System.out.println(stdClass.getDeclaredField("grade"));
    }
}

class Student extends Person {
    public int score;
    private int grade;
}

class Person {
    public String name;
}
```

## :point_right:调用方法

`Class`类提供了以下几个方法来获取`Method`：

- `Method getMethod(name, Class...)`：获取某个`public`的`Method`（包括父类）
- `Method getDeclaredMethod(name, Class...)`：获取当前类的某个`Method`（不包括父类）
- `Method[] getMethods()`：获取所有`public`的`Method`（包括父类）
- `Method[] getDeclaredMethods()`：获取当前类的所有`Method`（不包括父类）

```Java
public class Main {
    public static void main(String[] args) throws Exception {
        Class stdClass = Student.class;
        // 获取public方法getScore，参数为String:
        System.out.println(stdClass.getMethod("getScore", String.class));
        // 获取继承的public方法getName，无参数:
        System.out.println(stdClass.getMethod("getName"));
        // 获取private方法getGrade，参数为int:
        System.out.println(stdClass.getDeclaredMethod("getGrade", int.class));
    }
}

class Student extends Person {
    public int getScore(String type) {
        return 99;
    }
    private int getGrade(int year) {
        return 1;
    }
}

class Person {
    public String getName() {
        return "Person";
    }
}
```

# :point_right:注解

什么是注解（Annotation）？注解是放在Java源码的类、方法、字段、参数前的一种特殊“注释”：

注释会被编译器直接忽略，注解则可以被编译器打包进入class文件，因此，注解是一种用作标注的“元数据”。

```Java
@Resource("hello")
public class Hello {@Injectint n;

    @PostConstructpublic void hello(@Param String name) {
        System.out.println(name);
    }

    @Overridepublic String toString() {
        return "Hello";
    }
}
```

Java的注解可以分为三类：

第一类是由编译器使用的注解，例如：

- `@Override`：让编译器检查该方法是否正确地实现了覆写；
- `@SuppressWarnings`：告诉编译器忽略此处代码产生的警告。

第二类是由工具处理`.class`文件使用的注解，比如有些工具会在加载class的时候，对class做动态修改，实现一些特殊的功能。这类注解会被编译进入`.class`文件，但加载结束后并不会存在于内存中。这类注解只被一些底层库使用，一般我们不必自己处理。

第三类是在程序运行期能够读取的注解，它们在加载后一直存在于JVM中，这也是最常用的注解。

```Java
public class Hello {@Check(min=0, max=100, value=55)
    public int n;

    @Check(value=99)
    public int p;

    @Check(99) // @Check(value=99)public int x;

    @Checkpublic int y;
}
```

## :point_right:定义注解

我们总结一下定义`Annotation`的步骤：

第一步，用`@interface`定义注解：

```Plaintext
public @interface Report {
}
```

第二步，添加参数、默认值：

```Plaintext
public @interface Report {
    int type() default 0;
    String level() default "info";
    String value() default "";
}
```

把最常用的参数定义为`value()`，推荐所有参数都尽量设置默认值。

第三步，用元注解配置注解：

```Plaintext
@Target(ElementType.TYPE)
@Retention(RetentionPolicy.RUNTIME)
public @interface Report {
    int type() default 0;
    String level() default "info";
    String value() default "";
}
```

其中，必须设置`@Target`和`@Retention`，`@Retention`一般设置为`RUNTIME`，因为我们自定义的注解通常要求在运行期读取。一般情况下，不必写`@Inherited`和`@Repeatable`。

## :point_right:处理注解

Java的注解本身对代码逻辑没有任何影响。根据`@Retention`的配置：

- `SOURCE`类型的注解在编译期就被丢掉了；
- `CLASS`类型的注解仅保存在class文件中，它们不会被加载进JVM；
- `RUNTIME`类型的注解会被加载进JVM，并且在运行期可以被程序读取。

因此，我们只讨论如何读取`RUNTIME`类型的注解。

因为注解定义后也是一种`class`，所有的注解都继承自`java.lang.annotation.Annotation`，因此，读取注解，需要使用反射API。

```Java
@Target(ElementType.FIELD)
@Retention(RetentionPolicy.RUNTIME)
public @interface MyField {
    String description();
    int length();
}

// 使用注解
public class MyFieldTest {

    //使用我们的自定义注解
    @MyField(description = "用户名", length = 12)
    private String username;

    @Test
    public void testMyField(){

        // 获取类模板
        Class c = MyFieldTest.class;

        // 获取所有字段
        for(Field f : c.getDeclaredFields()){
            // 判断这个字段是否有MyField注解
            if(f.isAnnotationPresent(MyField.class)){
                MyField annotation = f.getAnnotation(MyField.class);
                System.out.println("字段:[" + f.getName() + "], 描述:[" + annotation.description() + "], 长度:[" + annotation.length() +"]");
            }
        }

    }
}
```

# Somenote

## defualt

```Java
public interface Person {
    default String getName(){
        return "我是默认姓名";
    }
    default String getId(){
        return "我是默认ID";
    }
}
```
