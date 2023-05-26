![](../images/line3.png)

### Primitive Data Types - Integers

<sub>[previous](../errors/README.md#user-content-errors) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../)</sub>

![](../images/line3.png)

Information can be read and written from computer memory, that we see as RAM (Random Access Memory).  It needs to read from somewhere in memory.  It reads from a **place** called an **object** which is a region of memory of a specific size that holds information of a data type.

There are [primitive data types](https://www.geeksforgeeks.org/cpp-data-types/) that can be used natively in C++ without loading other libraries.  Let's look at a few of them.

### Integer

[Integers](https://www.mathsisfun.com/whole-numbers.html) are whole numbers without a fractional component.  This can include both negative and positive numbers. How do we read and write to this data type?  We name this object space with a **variable** then assign the variable with the assignment operator `=` a value (such as `2019`).  In a statement, this would look like `year = 2019;`.  We have a varible called `year` and it stores the **integer** `2019`.

How is `42` represented in a computer.  It is represented as a [binary](https://www.computerhope.com/jargon/b/binary.htm) value.  The system we use day to day is the decimal system which is base 10.  We start at 0, got 9 then add a digit 1 then start at 0 again (1, 2, 3, 4, 5, 6, 7, 8, 9, 10 etc..)

Binary is base 2 so it starts at 0 then goes to 1 then adds a digit 1 then goes back to 0.  

A bit represents a binary number of `0` or `1`.  A byte represents 8 bits (`00100100` is an example of a byte of data).


| Decimal &nbsp; &nbsp;| Binary &nbsp; &nbsp; &nbsp; &nbsp;|
| ----------| -------------|
| 0 | 0 |
| 1 | 1 | 
| 2 | 10 |
| 3 | 11 |
| 4 | 100 |
| 5 | 101 |

An integer *typically* requires 4 bytes (32 bits) of memory enough space to hold 2<sup>(4 * 8)</sup>. or 2<sup>32</sup> which would represent a signed number of -`2147483648` to `2147483647`.

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

Right click on the solution and select **Add | New Project...** and select an **Empty Project** that is in **C++**.  Press the <kbd>Next</kbd> button.

![create new empty c++ project](images/newProject.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

Name the project `Primitives` and put it in your working project folder.  Press the <kbd>Create</kbd> button.

![call project Primitives](images/primitivesProj.png)

![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Right click on the **Primitives** project and **Add | New Item...** and call this item `Primitives.cpp`.  

![add Primitives.cpp file](images/addPrimitivesCPP.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Add comments to the top.  Multiline comments use `/*` to start the comments and `*/` to end them.  This way we can clearly explain what the cpp file is supposed to do. Also, we need `std::cout` so lest `#include <iostream>` so we can use this object class.

![add include and comments to .cpp](images/header.png)

![](../images/line2.png)

##### `Step 5.`\|`CPPOVR`| :small_orange_diamond:

Nonw instead of always typing `std::cout` we can put before our **Main()** function a `using` directive to state that when we are using `cout` we mean `std::cout`.  This eliminates the ability to use this name in our project though. Then lets add a `main()` function that will run first and create an integer variable called `Year`.  Inside that we will assign the value `2045`. 

![alt_text](images/coutIntBasic2.png)

![](../images/line2.png)

##### `Step 6.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond:


In C++, a variable is a named storage location in memory that holds a value, which can change during the program's execution. It is a way to store data that can be used or manipulated later in the program.

Variable names are chosen to describe the type of data stored in them and are usually defined by the programmer. Examples of types of data stored in variables include integers, floating point numbers, characters and strings.

In C++ we need to define the type with a type specifier, then a variable name.  We then use the assignment operator `=` and assign a literal value to the variable.

So when we initialize a variable we need to have the following components, we are declaring and defining the variable in one step:

`type-specifier variable_name = literal_value;`

You can also just declare a variable without defining it.  But it will need to be defined before it is used.

`type-spedifier variable_name; `

Memory is alocated based on the size required by the type. So in the case of an integer, typtically 4 bytes.

![alt_text](images/setAsStartup.png)

![](../images/line2.png)

##### `Step 7.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:
![alt_text](images/setAsStartup.png)
![alt_text](images/.png)

![](../images/line2.png)

##### `Step 8.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 9.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 10.`\|`CPPOVR`| :large_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 11.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 12.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 13.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 14.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 15.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond: 

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 16.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 17.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 18.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 19.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 20.`\|`CPPOVR`| :large_blue_diamond: :large_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 21.`\|`CPPOVR`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - ADD NEXT PAGE"> -->

![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../errors/README.md#user-content-errors)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../)|
|---|---|---|
