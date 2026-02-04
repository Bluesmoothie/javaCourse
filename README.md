# JAVA

## Summary

- [JAVA](#java)
	- [Summary](#summary)
	- [1. Variables](#1-variables)
		- [ 1.1 Declaration and assignment](#11-declaration-and-assignment)
		- [1.2 Strings concatenation](#12-strings-concatenation)
		- [1.3 Constants](#13-constants)
	- [2. Classes](#2-classes)
	- [3. Packages](#3-packages)
	- [4. Main function](#4-main-function)
	- [5. Comment](#5-comment)
	- [6. Compiling and executing](#6-compiling-and-executing)
	- [7. Access control](#7-access-control)
	- [8. Loops](#8-loops)
		- [8.1 For loops](#81-for-loops)
			- [8.1.1 For each loops](#811-for-each-loops)
		- [8.2 While loops](#82-while-loops)
			- [8.2.1 Do while loops](#821-do-while-loops)
		- [8.3 Continue](#83-continue)
		- [8.4 Break](#84-break)

## 1. Variables

###  1.1 Declaration and assignment

```java
String  str = "Hello World!";
boolean bool = true;
int     num = 42;
float   dec1 = 0.1
double  dec2 = 0.000001;
```

> [!IMPORTANT]
> String is an object, not a pure type

### 1.2 Strings concatenation

You can easily concatenate string and other type using the ```+``` operator

```java
final String    str = "Hello";
final String    user = "Jones";
final int       id = 42;
String          concatenate = str + " " + user + " " + id;
```

Here concatenate will be: ```Hello Jones 42```

### 1.3 Constants

```java
final int   CONSTNUM = 4242;
```

> [!NOTE]  
> Constants are nammed in capital

## 2. Classes

```java
public class    myClass {

}
```

> [!IMPORTANT]
> In Java, everything need to be in a class

## 3. Packages

A package is a group of classes

Declare a package with ```package```:

```java
package myPackage;
```

> [!IMPORTANT]
> This is the first line of every ```.java``` file

> [!IMPORTANT]
> The package and classes names follow the path  
> Ex: if the path is myApp/userManagment/userManagment.java  
> The package will be myApp.userManagment  
> The class in this file will be userManagment

## 4. Main function

The main class will be the entrypoint of your program

```java
public static void main(String[] args) {

}
```

## 5. Comment

```java
//  Single line comment
/** Multi-line
    comment */
```

## 6. Compiling and executing

Use ```javac``` to compile and ```java``` to execute

```bash
javac helloWorld
java helloWorld.helloWorld
> Hello World!
```

## 7. Access control

| Keyword           | Access level            |
|-------------------|-------------------------|
| public            | Program                 |
| protected         | Package and sub classes |
| package-protected | Package only            |
| private           | Class only              |

> [!NOTE]
> If not precised, the element get the access level of it's parent

## 8. Loops

### 8.1 For loops

```java
for(int i = 0; i < 10; ++i) {
     whatever();
}
```

Execute whatever 10 times

#### 8.1.1 For each loops

```java
for(int num: numArray) {
     whatever(num);
}
```

Execute whatever for each number in ```numArray```

### 8.2 While loops

```java
while(condition()) {
     whatever();
}
```

Execute whatever as long as ```condition()``` return is not 0

#### 8.2.1 Do while loops

```java
do {
     whatever();
} while (condition());
```

Same as ```while``` but evaluate the condition after the loop

### 8.3 Continue

```java
continue;
```

Go to the next loop iteration, ignoring if there is other instructions below

### 8.4 Break

```java
break;
```

Stop the loop prematurely
