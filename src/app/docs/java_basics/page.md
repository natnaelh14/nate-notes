---
title: Java basics
nextjs:
  metadata:
    title: Java basics
    description: Learn Java Essentials
---

## Introduction

![](/image/java/java-1.png)

![](/image/java/java-2.png)

**.class** is an intermediate format. It is a byte code.
**Byte code** is an instruction set meant for execution by the JVM.

You run Java using a Java Virtual Machine (JVM) and Java Runtime Edition (JRE).

![](/image/java/java-3.png)

It is only necessary if you are planning to develop in Java.

![](/image/java/java-4.png)

Windows, Macs, and Linux will have different Java Runtime Environments.

![](/image/java/java-5.png)

**Just In Time Compiler** – It is a selected optimization that the JVM does to convert byte code into direct machine level code that is run on the bare bones machine.

After Java 9, There is an option for **Ahead of Time Compilation (AOT)**. It converts intermediate code fully to native code before executing.

![](/image/java/java-6.png)

With C/C++, you don’t have those advantages.

Design goals of Java:

![](/image/java/java-7.png)

You can use **javac** to compile java code into (.class).

![](/image/java/java-8.png)

**java** command takes in the class name as an argument.

![](/image/java/java-9.png)

With newer versions, you can compile and run java code at the same time.

![](/image/java/java-10.png)

![](/image/java/java-11.png)

![](/image/java/java-12.png)

![](/image/java/java-13.png)

The keyword **main** is the special indicator that this is what start of the execution of a program.

![](/image/java/java-14.png)

## Primitive Types

Primitives are one of the few times where you don’t have to deal with objects in Java.
In Java, “Strings” are objects.

![](/image/java/java-15.png)

![](/image/java/java-16.png)

**Int** – 32-bit number
**Long** – 64-bit number
**Float** – 32-bit floating points
**Double** – 64-bit float points

![](/image/java/java-17.png)

![](/image/java/java-18.png)

A smaller data type takes up less space.
**Byte** – Min value (-128) and Max value (127)
**Short** – Min value (-32768) and Max value (32767)
**Int** - Min value (-2147483648) and Max value (2147483647)

![](/image/java/java-19.png)

![](/image/java/java-20.png)

![](/image/java/java-21.png)

![](/image/java/java-22.png)

Because it is more precise, the **double** is the default type for floating point numbers. It is the preferred data type to use.
The float data type can be specified as a numeric literal with a suffix of lowercase **f**, or uppercase**F**. The suffix is required if you are assigning a real number to a variable that was declared with a float type.

![](/image/java/java-23.png)

![](/image/java/java-24.png)

### Literals

It is when you define a value literally in your code. It is a way to specify a value inline.

![](/image/java/java-25.png)

![](/image/java/java-26.png)

## Static Typing

JavaScript has dynamic typing.

![](/image/java/java-27.png)

Allowed Conversion:
Short -> int,
Byte -> int.
Float -> int

![](/image/java/java-28.png)

## Type Promotion

![](/image/java/java-29.png)

## Casting

![](/image/java/java-30.png)

![](/image/java/java-31.png)

![](/image/java/java-32.png)

![](/image/java/java-33.png)

## Method

Method is a collection statements, one or more, that perform an operation.

![](/image/java/java-34.png)

**Public** – it is available to the outside world.
**Static** – it can be called using the class name.
**Void** – it is the return type.

![](/image/java/java-35.png)

![](/image/java/java-36.png)

## Method Overloading

![](/image/java/java-37.png)

![](/image/java/java-38.png)

You can assign strong access privilege, but you can not make it weaker.

![](/image/java/java-178.png)

## Switch Statement

![](/image/java/java-39.png)

Starting with Java 14, You can return the value of a switch statement.
**break** is not required here.

![](/image/java/java-40.png)

## If/else block

![](/image/java/java-41.png)
![](/image/java/java-42.png)
![](/image/java/java-43.png)
![](/image/java/java-44.png)

## Loop

![](/image/java/java-45.png)
![](/image/java/java-46.png)
![](/image/java/java-47.png)
![](/image/java/java-48.png)
![](/image/java/java-49.png)
![](/image/java/java-50.png)
![](/image/java/java-51.png)
![](/image/java/java-52.png)

## Parse

![](/image/java/java-53.png)

## Try statement

![](/image/java/java-54.png)

## New keyword

![](/image/java/java-55.png)

## Scanner

![](/image/java/java-56.png)

## Object Oriented Programming

It is sometimes called class-based programming.

![](/image/java/java-57.png)

![](/image/java/java-58.png)

![](/image/java/java-59.png)

![](/image/java/java-60.png)

![](/image/java/java-61.png)

Class Names follow pascal case. Member Variables follow camel case.

![](/image/java/java-62.png)

When you create a new variable, the Java runtime will allocate space for the variable.
But when you initialize, I will allocate memory space for the member variables (instance variables) of the class. The memory allocation happens at runtime.

![](/image/java/java-63.png)

## Packages

![](/image/java/java-167.png)

There is no relationship between **parent** and **child** packages.

**import** is required to use a class from a different package.

![](/image/java/java-168.png)

## Access Modifiers

They encapsulate and restrict access to member variables and methods.

![](/image/java/java-64.png)

A class could be thought of as a powerful way to find a data type, like String.

![](/image/java/java-65.png)

• When there is no modifier access specified, Java will automatically.

• The default access modifier is **package private**. It acts like public, if in the same package.

• It acts like private to other packages.

![](/image/java/java-66.png)

![](/image/java/java-67.png)

![](/image/java/java-169.png)

### Best Practices

![](/image/java/java-170.png)

## Encapsulation

![](/image/java/java-68.png)

![](/image/java/java-144.png)

An application programming interface, **API** is a public contract that tells other class members how to use the class.

## Getter and Setter

![](/image/java/java-69.png)

![](/image/java/java70.png)

### Setter

![](/image/java/java-71.png)

### Getter

![](/image/java/java-72.png)

## Variable Shadowing

The **this** reference refers to the instance the method will be run on.

![](/image/java/java-73.png)

## Constructor

A constructor function is created for you implicitly by Java.

![](/image/java/java-74.png)

![](/image/java/java-75.png)

![](/image/java/java-76.png)

![](/image/java/java-77.png)

The call to **this** must be the first statement in the constructor body.

![](/image/java/java-78.png)

### Copy Constructor

Copy constructor is a constructor which takes in as an argument an instance of that same class and copies over the member variables.

![](/image/java/java-165.png)

## Reference Vs Object Vs Instance Vs Class

![](/image/java/java-79.png)

![](/image/java/java-80.png)

![](/image/java/java-81.png)

![](/image/java/java-82.png)

![](/image/java/java-166.png)

• Java uses call by value.

• Any value passed as parameters is "copied" to the method arguments.

• If the argument is an object reference, the reference is copied.

• The reference copy points to the same instance as the source object reference. So if you change the class member value, it will be propagated everywhere else.

## Static

The **static** keyword is used when you need to define a class member as independent from any object instance.

### Static Vs Instance Variables

![](/image/java/java-83.png)

![](/image/java/java-84.png)

![](/image/java/java-85.png)

**Static variables** are shared between instances.

![](/image/java/java-86.png)

![](/image/java/java-87.png)

![](/image/java/java-88.png)

![](/image/java/java-89.png)

### Static Vs Instance Methods

![](/image/java/java-90.png)

**Static methods** don’t need an instance to be created. That is why the **main()** method is a static method.

![](/image/java/java-91.png)

![](/image/java/java-92.png)

![](/image/java/java-93.png)

The method **bark** is just an instance method, since it doesn’t have the **static** keyword.

![](/image/java/java-94.png)

## Final

```js
    final String name = "Acme Inc";
```

![](/image/java/java-171.png)

## Nested Classes

### Static Inner Classes

![](/image/java/java-172.png)

### Inner Class (Non-Static Nested Class)

![](/image/java/java-173.png)

### Local Class

![](/image/java/java-174.png)

### Anonymous Class

![](/image/java/java-175.png)

## Local Classes and Closure Variables

What needs to happen for an outer variable to be accessed in a local class?

It has to be final or effectively final.

![](/image/java/java-176.png)

## POJO

![](/image/java/java-95.png)

![](/image/java/java-96.png)

## Annotation

![](/image/java/java-97.png)

**Override** is one of the most common annotations we will use.

![](/image/java/java-98.png)

![](/image/java/java-99.png)

Every object, when passed to system.out.println() will have the toString() method implicitly executed, if you have created such a method in your class.

![](/image/java/java-100.png)

![](/image/java/java-101.png)

## Record Type

![](/image/java/java-102.png)

![](/image/java/java-103.png)

![](/image/java/java-104.png)

When the field is **final**, it means it can’t be modified.

![](/image/java/java-105.png)

![](/image/java/java-106.png)

![](/image/java/java-107.png)

![](/image/java/java-108.png)

Instead of the above utilizing POJO, with record, You can just use this block of code and have access to **toString()**, and getter/setter equivalent.

![](/image/java/java-109.png)

## Inheritance

It is a way to organize classes into a parent child hierarchy, which lets the child inherit (re-use) fields and methods from its parents.
**Extends** – using extends specifies the superclass (or the parent class) of the class we are declaring.

![](/image/java/java-177.png)

![](/image/java/java-110.png)

![](/image/java/java-111.png)

![](/image/java/java-112.png)

We have to pass arguments to super(), since Animal class does not have any default constructor.

![](/image/java/java-113.png)

![](/image/java/java-114.png)

The **this()** keyword is called line 11 with four arguments.
Even if **toString()** is defined in Animal class, the **toString()** in Dog class will override it.

![](/image/java/java-115.png)

![](/image/java/java-116.png)

The modified, **protected**, says that any class that is a sub-class can access this field. It is called conditional encapsulation. It also means that any classes in the same package will also have access.

![](/image/java/java-117.png)

## Java.Lang.Object

![](/image/java/java-118.png)

![](/image/java/java-119.png)

## This Vs Super

![](/image/java/java-120.png)

![](/image/java/java-121.png)

If we don’t use the super keyword as shown in the MainClass, it becomes a recursive call.

![](/image/java/java-122.png)

![](/image/java/java-123.png)

![](/image/java/java-124.png)

The problem the **BAD** example is the duplicated code. Using constructor chaining, you can avoid code duplication.

![](/image/java/java-125.png)

## Method Overloading/Method Overriding

![](/image/java/java-126.png)

Java developers often refer to method overloading, as compile-time polymorphism.
This means the compiler is determining the right method to call, based on the method name and argument list.

![](/image/java/java-127.png)

![](/image/java/java-128.png)

![](/image/java/java-129.png)

![](/image/java/java-130.png)

![](/image/java/java-131.png)

## Text Block

![](/image/java/java-132.png)

![](/image/java/java-133.png)

**%d** is called format specifier.

![](/image/java/java-134.png)

![](/image/java/java-135.png)

![](/image/java/java-136.png)

![](/image/java/java-137.png)

![](/image/java/java-138.png)

![](/image/java/java-139.png)

![](/image/java/java-140.png)

## Composition

![](/image/java/java-141.png)

![](/image/java/java-142.png)

![](/image/java/java-143.png)

## Polymorphism

Simply stated, Polymorphism means many forms.

![](/image/java/java-145.png)

**Factory methods** give us a way to get an object, without having to know the details of having to create a new one or specify the exact class we want.

## Casting

**LVTI** – Local Variable Type Inference

![](/image/java/java-146.png)

![](/image/java/java-147.png)

## InstanceOf

![](/image/java/java-148.png)

![](/image/java/java-149.png)

![](/image/java/java-150.png)

## Import

![](/image/java/java-151.png)

## Array

An **array** is a data structure, that allows you to store a sequence of values, all of the same type.
When you declare an array, it doesn’t automatically allocate memory to it.

![](/image/java/java-152.png)

Because the values are specified, the length of the array can be determined,so we don't specify the size of the square brackets.

![](/image/java/java-154.png)

![](/image/java/java-155.png)

![](/image/java/java-156.png)

![](/image/java/java-157.png)

```js
        int[] firstTen = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        for (int element : firstTen) {
            System.out.println(element + " ");
        }
```

![](/image/java/java-158.png)

```js
        import java.util.Arrays;
        ...
        int[] firstTen = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        System.out.println(Arrays.toString(firstTen));
```

### Binary Search

![](/image/java/java-159.png)

![](/image/java/java-160.png)

![](/image/java/java-161.png)

```js
        String[] sArray = {"Able", "Jane", "Mark", "Ralph", "David"};
        Arrays.sort(sArray);
        if(Arrays.binarySearch(sArray, "Mark") >= 0 ){
            System.out.println("Found Mark in the list.");
        }
        //Found Mark in the list.
```

### Equality of Arrays

```js
        int[] s1 = {1, 2, 3, 4, 5};
        int[] s2 = {1, 2, 3, 4, 5};
        if(Arrays.equals(s1, s2)) {
            System.out.println("Arrays are equal.");
        }
        //Arrays are equal.
```

### Reference Types vs Value Types

```js

        //Reference is the address to the object in memory, but not the object itself.
        int[] myIntArray = new int[5];
        int[] anotherArray = myIntArray;
        System.out.println("myIntArray = " + Arrays.toString(myIntArray));
        System.out.println("anotherArray = " + Arrays.toString(anotherArray));
        anotherArray[0] = 1;
        System.out.println("after change myIntArray = " + Arrays.toString(myIntArray));
        System.out.println("after change anotherArray = " + Arrays.toString(anotherArray));
        // myIntArray = [0, 0, 0, 0, 0]
        // anotherArray = [0, 0, 0, 0, 0]
        // after change myIntArray = [1, 0, 0, 0, 0]
        // after change anotherArray = [1, 0, 0, 0, 0]

```

### Variable Argument

![](/image/java/java-162.png)

### Multidimensional Array

![](/image/java/java-153.png)

![](/image/java/java-163.png)

## List

![](/image/java/java-164.png)

```js
record GroceryItem (String name, String type, int count) {
    public GroceryItem(String name) {
        this(name, "DAIRY", 10);
    }
}
public class Main {
    public static void main(String[] args) {
        GroceryItem[] groceryArray = new GroceryItem[3];
        groceryArray[0] = new GroceryItem("milk");
        groceryArray[1] = new GroceryItem("apples", "PRODUCE", 6);
        groceryArray[2] = new GroceryItem("oranges");
        System.out.println(Arrays.toString(groceryArray));
        //<> is called a diamond operator so that it can infer the array type.
        ArrayList<GroceryItem> groceryList = new ArrayList<>();
        groceryList.add(new GroceryItem("avocado"));
        groceryList.add(new GroceryItem("milk"));
        groceryList.add(new GroceryItem("cake"));
        groceryList.set(0, new GroceryItem("juice"));
        groceryList.remove(2);
        System.out.println(groceryList);
    }
}
```
