![](../images/line3.png)

### Primitive Data Types - Bools and Unsigned Ints

<sub>[previous](../fractions/README.md#user-content-primitive-data-types---fractions) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../)</sub>

![](../images/line3.png)

Now lets look at the data type called [bool](https://www.geeksforgeeks.org/c-data-types/). 
> Boolean: Boolean data type is used for storing boolean or logical values. A boolean variable can store either true or false. Keyword used for boolean data type is bool.- [geeksforgeeks.org](https://www.geeksforgeeks.org/c-data-types/)

Now we can use the literal value `true` and `false` and a single bit is needed so we have `0` for `false` and `1` for true (or any non 0 value). 

The Unreal 4 coding standards say:
> Boolean variables must be prefixed by b (for example, bPendingDestruction, or bHasFadedIn).  - [Unreal Manual](https://docs.unrealengine.com/en-us/Programming/Development/CodingStandard)

Note, that even if a boolean is a single bit the smallest amount of memory we can access is a byte.  So a bool takes a byte which wastes 7 bits.  There are ways of masking other types to be more efficient and we will show you that in Unreal later.

In C++, the unsigned int data type is used to represent whole numbers (integers) that can only be positive or zero. The "unsigned" part means that it doesn't include negative values.

Imagine you have a variable of type `unsigned int`. This variable can hold non-negative whole numbers, including zero. It cannot store negative numbers.

For example, if you declare an `unsigned int` variable called `X` and assign it a value of `-5`, it means that X can only store positive whole numbers or zero. You can perform various arithmetic operations on x, such as addition, subtraction, multiplication, and division, just like you would with regular integers.

One key advantage of using unsigned int is that it allows you to represent larger positive numbers than a regular int data type. The unsigned int uses the same amount of memory as a regular int but can store larger values because it doesn't need to allocate space for negative numbers.

However, it's important to note that using unsigned int also has some limitations. Since it doesn't support negative numbers, operations like subtracting a larger number from a smaller number may result in unexpected behavior. In addition, division between two unsigned int values may truncate the decimal part, as it produces an integer result.

|Type|Typical Bit Width|Typical Range|
|:----|:----|:----|
|unsigned int|4bytes|0 to 4294967295|
|signed int|4bytes|-2147483648 to 2147483647|

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

Add a comment for a bool section.  Add an appropriate title for this section. Then use the literal `true` to set the bool variable `bIsGood`.  Now when you output it to the stream it will not use the **string** `true` but will instead represent `true` with the **integer** `1`.

![set true bool and print to console](images/boolAs1.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

Now switch the value to `false` to represent the only other state of a boolean.  Notice that it outputs it to the console as **int** `0`.

![alt_text](images/falseBool.png)

![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 5.`\|`CPPOVR`| :small_orange_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 6.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 7.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

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

| [previous](../fractions/README.md#user-content-primitive-data-types---fractions)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../)|
|---|---|---|
