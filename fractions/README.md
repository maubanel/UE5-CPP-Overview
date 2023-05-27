![](../images/line3.png)

### Primitive Data Types - Fractions

<sub>[previous](../operators/README.md#user-content-arithmetic-operators) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../)</sub>

![](../images/line3.png)

We are going to introduce a new data type called a **double** floating point number.
> Double Floating Point: Double Floating Point data type is used for storing double precision floating point values or decimal values. Keyword used for double floating point data type is double. Double variables typically requires 8 bytes of memory space. - [geeksforgeeks.org](https://www.geeksforgeeks.org/cpp-data-types/?ref=gcse)

Notice that it says **typically**.  It is very important to understand that different platforms may have different sizes for the same named data types.  Always make sure you test your assumptions on ALL platforms you want to support.

What does 8 bytes mean?  A **byte** is 8 **bits**.  A bit is a single binary value (can be either `0` or `1`).  So if we have one **byte** it can store 8 **bits**.  So what does this mean in decimals?  We need to look at 2 to the power of 8 (2 ^ 8 or 2\*2\*2\*2\*2\*2\*2\*2).  Type `2 ^ 8` in a calculator and you will see that is **256**.  So a byte can hold an **integer** value of a number with **256** discrete values.  Now since 0 counts as a number a byte can hold any integer from `0` to `255`.  Why **255**?  Because 0 counts as a value.  We we have 256 discrete values.

So a double uses one bit for the sign (positive or negative), 11 bits for the exponent and 52 bits for the value (8 bytes =  8 \* 8 bits = 64 bits ). 

We are also going to introduce a new data type called [float](https://www.geeksforgeeks.org/cpp-data-types/?ref=gcse).
> Floating Point: Floating Point data type is used for storing single precision floating point values or decimal values. Keyword used for floating point data type is float. Float variables typically requires 4 byte of memory space. - [geeksforgeeks.org](https://www.geeksforgeeks.org/cpp-data-types/?ref=gcse)

Notice that it says **typically**.  It is very important to understand that different platforms may have different sizes for the same named data types.  

Now when do we use floats and when do we use doubles?  In games audio samples tend to use floats and in 3-D our points are usually stored in floats as well in **x, y, z Space** as there are so many of them.  The increase in precision is not offset by the huge size increase in RAM.  So floats are used when possible in games. In games where possible we use floats instead of doubles to save on memory (RAM).

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

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

| [previous](../operators/README.md#user-content-arithmetic-operators)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../)|
|---|---|---|
