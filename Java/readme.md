##[MainPage](../readme.md)/Java  

-
```java
public class VariableDemo{
	public static void main(String[] args){
		
	}
}
```
**calss**:​ 表示定义一个`类`。创建一个类。  

**类**：Java项目最基本的组成单元，一个完整的Java项目有可能会有成千上万个类来组成的。  

class后面跟随的就是这个类的名字，简称：类名。  

类的实现包括两部分：`类的声明`和`类体`。  

**类体**:包括类声明之后的*一对大括号{ }以及它们之间的内容*成为类体，大括号之间的内容称为类体的内容。  

类体分为两部分：`变量的声明`和`方法的定义`。  



```
class 类名{

        变量的声明;

        方法的定义;

    }
```

"VariableDemo"后的大括号表示这个类的范围。  

**public**：表内示程序的访问权限，表示的是任何的场合可以被引用。  

**main**:Java应用程序的入口方法(JVM找到这个程序的入口)，将其声明为public即对外公开，因此JVM便能直接调用它。  
每一个应用程序都必须包含一个main()方法，含有main()方法的类称为主类。  
**static**  
**void**  

###变量 
  - **变量**分为`成员变量`和`局部变量`  

    - **成员变量**：是变量声明部分声明的变量。（成员变量分为：`实例变量`、`类变量`。用*static*修饰的为类变量（*static变量，也叫静态变量*），否则为实例变量）  

    - **局部变量**：在方法体中声明的变量和方法的参数。  

- **变量的有效范围**
  - `成员变量`在整个类中都有效。
  - `局部变量`只在声明它的方法内有效
  - 方法参数在整个方法内有效。
  - 方法内的局部变量从声明它的位置之后开始有效。  

- **成员变量的隐藏**  
    如果局部变量的名字和成员变量的名字相同，则成员变量被隐藏（即这个成员变量在这个方法内暂时失效）。
  

###键盘录入
```java
//1.导包，先找到Scanner这个类在哪(idea在进行步骤2后会自动进行导包)
import java.util.Scanner;
public class class1 {
    public static void main(String[] args) {
        //2.创建对象，申明一下，我准备开始用Scanner这个类了。
        Scanner sc = new Scanner(System.in);
        System.out.println("请输入一个数字");
		//3.接收数据
        int i = sc.nextInt();
        System.out.println(i);
    }
}
```
```java
import java.util.Scanner;
```
导包的动作必须出现在类的定义上  
```java
Scanner sc = new Scanner(System.in);
```
此行代码中只有sc为变量名，可变，其余均不可变  
```java
int i = sc.nextInt();
```
其中只有后半为接收数据，前半意为将接收的数据赋值给变量i。此行代码中只有i为变量名，可变，其余均不可变  

### 运算符及表达式  

- **运算符**    
对常量或者变量进行操作的符号  

| 运算符 | 说明 |
|-------|------|
| + | 加 |
| - | 减 |
| * | 乘 |
| / | 除 |
| % | 取余数 |  

```java
/*
1.整数相除结果只能得到整除，如果结果想要是小数，必须要有小数参数。
2.小数直接参与运算，得到的结果有可能是不精确的。*/
System.out.println( 10 / 3);//3
System.out.println(10.0 / 3);//3.3333333333333335
```

```java
/*%：取模、取余。
   他做的也是除法运算，只不过获取的是余数而已。*/
System.out.println(10 % 2);//0
System.out.println(10 % 3);//1  
```








