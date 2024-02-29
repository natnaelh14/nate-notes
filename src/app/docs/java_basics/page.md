---
title: Java basics
nextjs:
  metadata:
    title: Java basics
    description: Learn Java Essentials
---

## Introduction

![](/image/java-1.png)

![](/image/java-2.png)

**.class** is an intermediate format. It is a byte code.
**Byte code** is an instruction set meant for execution by the JVM.

You run Java using a Java Virtual Machine (JVM) and Java Runtime Edition (JRE).

![](/image/java-3.png)

It is only necessary if you are planning to develop in Java.

![](/image/java-4.png)

Windows, Macs, and Linux will have different Java Runtime Environments.

![](/image/java-5.png)

**Just In Time Compiler** – It is a selected optimization that the JVM does to convert byte code into direct machine level code that is run on the bare bones machine.

After Java 9, There is an option for **Ahead of Time Compilation (AOT)**. It converts intermediate code fully to native code before executing.

![](/image/java-6.png)

With C/C++, you don’t have those advantages.

Design goals of Java:

![](/image/java-7.png)

You can use **javac** to compile java code into (.class).

![](/image/java-8.png)

**java** command takes in the class name as an argument.

![](/image/java-9.png)

With newer versions, you can compile and run java code at the same time.

![](/image/java-10.png)

![](/image/java-11.png)

![](/image/java-12.png)

![](/image/java-13.png)

The keyword **main** is the special indicator that this is what start of the execution of a program.

![](/image/java-14.png)

## Primitive Types

Primitives are one of the few times where you don’t have to deal with objects in Java.
In Java, “Strings” are objects.

![](/image/java-15.png)

![](/image/java-16.png)

**Int** – 32-bit number
**Long** – 64-bit number
**Float** – 32-bit floating points
**Double** – 64-bit float points

![](/image/java-17.png)

![](/image/java-18.png)

A smaller data type takes up less space.
**Byte** – Min value (-128) and Max value (127)
**Short** – Min value (-32768) and Max value (32767)
**Int** - Min value (-2147483648) and Max value (2147483647)

![](/image/java-19.png)

![](/image/java-20.png)

![](/image/java-21.png)

![](/image/java-22.png)

Because it is more precise, the **double** is the default type for floating point numbers. It is the preferred data type to use.
The float data type can be specified as a numeric literal with a suffix of lowercase **f**, or uppercase**F**. The suffix is required if you are assigning a real number to a variable that was declared with a float type.

![](/image/java-23.png)

![](/image/java-24.png)

### Literals

It is when you define a value literally in your code. It is a way to specify a value inline.

![](/image/java-25.png)

![](/image/java-26.png)

## Static Typing

JavaScript has dynamic typing.

![](/image/java-27.png)

Allowed Conversion:
Short -> int,
Byte -> int.
Float -> int

![](/image/java-28.png)

## Type Promotion

![](/image/java-29.png)

## Casting

![](/image/java-30.png)

![](/image/java-31.png)

![](/image/java-32.png)

![](/image/java-33.png)

## Method

Method is a collection statements, one or more, that perform an operation.

![](/image/java-34.png)

**Public** – it is available to the outside world.
**Static** – it can be called using the class name.
**Void** – it is the return type.

![](/image/java-35.png)

![](/image/java-36.png)

## Method Overloading

![](/image/java-37.png)

![](/image/java-38.png)

## Switch Statement

![](/image/java-39.png)

Starting with Java 14, You can return the value of a switch statement.
**break** is not required here.

![](/image/java-40.png)

## If/else block

![](/image/java-41.png)
![](/image/java-42.png)
![](/image/java-43.png)
![](/image/java-44.png)

## Loop

![](/image/java-45.png)
![](/image/java-46.png)
![](/image/java-47.png)
![](/image/java-48.png)
![](/image/java-49.png)
![](/image/java-50.png)
![](/image/java-51.png)
![](/image/java-52.png)

## Parse

![](/image/java-53.png)

## Try statement

![](/image/java-54.png)

## New keyword

![](/image/java-55.png)

## Scanner

![](/image/java-56.png)

## Object Oriented Programming

It is sometimes called class-based programming.

![](/image/java-57.png)

![](/image/java-58.png)

![](/image/java-59.png)

![](/image/java-60.png)

![](/image/java-61.png)

Class Names follow pascal case. Member Variables follow camel case.

![](/image/java-62.png)

When you create a new variable, the Java runtime will allocate space for the variable.
But when you initialize, I will allocate memory space for the member variables (instance variables) of the class. The memory allocation happens at runtime.

![](/image/java-63.png)

## Access Modifiers

![](/image/java-64.png)

A class could be thought of as a powerful way to find a data type, like String.

![](/image/java-65.png)

When there is no modifier access specified, Java will automatically.

![](/image/java-66.png)

![](/image/java-67.png)

## Encapsulation

![](/image/java-68.png)

## Getter and Setter

![](/image/java-69.png)

![](/image/java70.png)

### Setter

![](/image/java-71.png)

### Getter

![](/image/java-72.png)

## Variable Shadowing

The **this** reference refers to the instance the method will be run on.

![](/image/java-73.png)

## Constructor

A constructor function is created for you implicitly by Java.

![](/image/java-74.png)

![](/image/java-75.png)

![](/image/java-76.png)

![](/image/java-77.png)

The call to **this** must be the first statement in the constructor body.

![](/image/java-78.png)

## Reference Vs Object Vs Instance Vs Class

![](/image/java-79.png)

![](/image/java-80.png)

![](/image/java-81.png)

![](/image/java-82.png)

## Static Vs Instance Variables

![](/image/java-83.png)

![](/image/java-84.png)

![](/image/java-85.png)

**Static variables** are shared between instances.

![](/image/java-86.png)

![](/image/java-87.png)

![](/image/java-88.png)

![](/image/java-89.png)

## Static Vs Instance Methods

![](/image/java-90.png)

**Static methods** don’t need an instance to be created.

![](/image/java-91.png)

![](/image/java-92.png)

![](/image/java-93.png)

The method **bark** is just an instance method, since it doesn’t have the **static** keyword.

![](/image/java-94.png)

## POJO

![](/image/java-95.png)

![](/image/java-96.png)

## Annotation

![](/image/java-97.png)

**Override** is one of the most common annotations we will use.

![](/image/java-98.png)

![](/image/java-99.png)

Every object, when passed to system.out.println() will have the toString() method implicitly executed, if you have created such a method in your class.

![](/image/java-100.png)

![](/image/java-101.png)

## Record Type

![](/image/java-102.png)

![](/image/java-103.png)

![](/image/java-104.png)

When the field is **final**, it means it can’t be modified.

![](/image/java-105.png)

![](/image/java-106.png)

![](/image/java-107.png)

![](/image/java-108.png)

Instead of the above utilizing POJO, with record, You can just use this block of code and have access to **toString()**, and getter/setter equivalent.

![](/image/java-109.png)

## Inheritance

It is a way to organize classes into a parent child hierarchy, which lets the child inherit (re-use) fields and methods from its parents.
**Extends** – using extends specifies the superclass (or the parent class) of the class we are declaring.

![](/image/java-110.png)

![](/image/java-111.png)

![](/image/java-112.png)

We have to pass arguments to super(), since Animal class does not have any default constructor.

![](/image/java-113.png)

![](/image/java-114.png)

The **this()** keyword is called line 11 with four arguments.
Even if **toString()** is defined in Animal class, the **toString()** in Dog class will override it.

![](/image/java-115.png)

![](/image/java-116.png)

The modified, **protected**, says that any class that is a sub-class can access this field. It is called conditional encapsulation. It also means that any classes in the same package will also have access.

![](/image/java-117.png)

## Java.Lang.Object

![](/image/java-118.png)

![](/image/java-119.png)

## This Vs Super

![](/image/java-120.png)

![](/image/java-121.png)

If we don’t use the super keyword as shown in the MainClass, it becomes a recursive call.

![](/image/java-122.png)

![](/image/java-123.png)

![](/image/java-124.png)

The problem the **BAD** example is the duplicated code. Using constructor chaining, you can avoid code duplication.

![](/image/java-125.png)

## Method Overloading/Method Overriding

![](/image/java-126.png)

Java developers often refer to method overloading, as compile-time polymorphism.
This means the compiler is determining the right method to call, based on the method name and argument list.

![](/image/java-127.png)

![](/image/java-128.png)

![](/image/java-129.png)

![](/image/java-130.png)

![](/image/java-131.png)

## Text Block

![](/image/java-132.png)

![](/image/java-133.png)

**%d** is called format specifier.

![](/image/java-134.png)

![](/image/java-135.png)

![](/image/java-136.png)

![](/image/java-137.png)

![](/image/java-138.png)

![](/image/java-139.png)

![](/image/java-140.png)

## Composition

![](/image/java-141.png)

![](/image/java-142.png)

![](/image/java-143.png)

## Encapsulation

![](/image/java-144.png)

An application programming interface, **API** is a public contract that tells other class members how to use the class.

## Polymorphism

Simply stated, Polymorphism means many forms.

![](/image/java-145.png)

**Factory methods** give us a way to get an object, without having to know the details of having to create a new one or specify the exact class we want.

## Casting

**LVTI** – Local Variable Type Inference

![](/image/java-146.png)

![](/image/java-147.png)

## InstanceOf

![](/image/java-148.png)

![](/image/java-149.png)

![](/image/java-150.png)

## Import

![](/image/java-151.png)

## Array

When you declare an array, it doesn’t automatically allocate memory to it.

![](/image/java-152.png)

## Multidimensional Array

![](/image/java-153.png)

```js
/** @type {import('@tailwindlabs/lorem').ipsum} */
export default {
  lorem: 'ipsum',
  dolor: ['sit', 'amet', 'consectetur'],
  adipiscing: {
    elit: true,
  },
}
```
