# Java-task4
作业4-空间中两点的距离

## 一、作业要求
&emsp;&emsp;求三维空间中两个给定点的距离。

## 二、解题思路
1. 设置类（task）是每一个点的坐标。建立三个成员变量（x,y,z）来存三个坐标量。设置构造函数，初始化三个坐标数值。
2. 设置方法（calc），根据公式计算两个点之间的距离，输出运算结果。
3. 设置主函数，创建两个task对象，使用构造函数赋值，调用计算公式，计算并显示结果。
4. 为了使运行结果更加直观，添加show函数用来显示点坐标。

## 三、关键代码
1. 设置成员变量和构造函数。
```java
    double x;
    double y;
    double z;
    public task(double a,double b,double c){
        x = a;
        y = b;
        z = c;
    }
```
2. calc方法，根据公式计算。该方法通过引入另外一个对象作为变量的方式，在两个对象之间做运算。分别求出两个坐标的x,y,z之差，平方求和，开根号。
```java
    public double calc(task a){
        double h;
        h = Math.sqrt((a.x - this.x)*(a.x - this.x)+(a.y - this.y)*(a.y - this.y)+(a.z - this.z)*(a.z - this.z));
        System.out.println("结果为"+h);
        return h;
    }
```
3. 设置主函数，初始化两个对象的成员变量，调用函数，计算求值，显示。
```java
    public static void main(String[] args){
        task port1 = new task(1,2,3);
        task port2 = new task(4,5,6);
        t1.show();
        t2.show();
        t1.calc(t2);
```
