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

```java
package myPackage;
```

Use this at the start of each file to name your package

> [!IMPORTANT]
> The package and classes names follow the path  
> Ex: if the path is myApp/userManagment/userManagment.java  
> The package will be myApp.userManagment  
> The class in this file will be userManagment

## 4. Main function

The main class will be the entrypoint of your program

```java
public static void	main(String[] args) {

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
