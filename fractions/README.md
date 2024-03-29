![](../images/line3.png)

### Primitive Data Types - Fractions

<sub>[previous](../operators/README.md#user-content-arithmetic-operators) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../bools/README.md#user-content-primitive-data-types---bools-and-unsigned-ints)</sub>

![](../images/line3.png)

We are going to introduce a new data type called a **double** floating point number.
> Double Floating Point: Double Floating Point data type is used for storing double precision floating point values or decimal values. Keyword used for double floating point data type is double. Double variables typically requires 8 bytes of memory space. - [geeksforgeeks.org](https://www.geeksforgeeks.org/cpp-data-types/?ref=gcse)

Notice that it says **typically**.  It is very important to understand that different platforms may have different sizes for the same named data types.  Always make sure you test your assumptions on ALL platforms you want to support.

What does 8 bytes mean?  A **byte** is 8 **bits**.  A bit is a single binary value (can be either `0` or `1`).  So if we have one **byte** it can store 8 **bits**.  So what does this mean in decimals?  We need to look at 2 to the power of 8 (2 ^ 8 or 2\*2\*2\*2\*2\*2\*2\*2).  Type `2 ^ 8` in a calculator and you will see that is **256**.  So a byte can hold an **integer** value of a number with **256** discrete values.  Now since 0 counts as a number a byte can hold any integer from `0` to `255`.  Why **255**?  Because 0 counts as a value.  We we have 256 discrete values.

So a double uses one bit for the sign (positive or negative), 11 bits for the exponent and 52 bits for the value (8 bytes =  8 \* 8 bits = 64 bits ). 

We are also going to introduce a new data type called [float](https://www.geeksforgeeks.org/cpp-data-types/?ref=gcse).
> Floating Point: Floating Point data type is used for storing single precision floating point values or decimal values. Keyword used for floating point data type is float. Float variables typically requires 4 byte of memory space. - [geeksforgeeks.org](https://www.geeksforgeeks.org/cpp-data-types/?ref=gcse)

Notice that it says **typically**.  It is very important to understand that different platforms may have different sizes for the same named data types.  

Now when do we use floats and when do we use doubles?  In games audio samples tend to use floats and in 3-D our points are usually stored in floats as well in **x, y, z Space** as there are so many of them.  The increase in precision is not offset by the huge size increase in RAM.  So floats are used when possible in games to save memory.

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

So lets create a new variable of type `double PercentChanceOfRain` and lets give it a silly double literal of `664433.89998999;`.  Notice that when we print it out it rounds the number and doesn't show the entire decimal number stored. Please note than any number we write with a decimal point (yes, even `3.`) is of type **double**. Also note that what it is printing to the console is not how it is represented in memory on the computer.  Lets fix that to the best of our abilities.

![double data type](images/doubleExample.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

Now based on the size of the double on my computer how many numbers can the scientific notation of a fractional [significand](https://en.wikipedia.org/wiki/Scientific_notation) hold?<br><br> 

`245 E 23` with `245` being the `significand` and `23` being the `exponent`.

It can store only so many digits.  We can demonstrate this by including the `<limits>` library to see how many total **base 10** digits this can hold.  Add to the after the first **include** `#include <limits>`.

![add <limits>](images/addLimits.png)

![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

 We use `std::numeric_limits<double>::max_digits10` to find out how many significand values it can hold which will determine the precision of the number.  Notice that we can be accurate up to `17` digits in base 10 numbers (remember the computer is storing this in binary).

![17 significand](images/doublesignificand.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now `cout` has a static function (will explain later) called `cout::set_precision(number_of_places)`.  This will show a floating point value with 17 numbers (not including the decimal `.` point). In this case we will show to the above precision.  Please notice that the last fractional parts are not identical to the number we set it to. We set it to `665533.89998899` and it ends up being `665533.89998899004`.

To read more look at [Floating-point error mitigation](https://en.wikipedia.org/wiki/Floating-point_error_mitigation) .

![adjust accuracy](images/doubleAccuracy.png)

![](../images/line2.png)

##### `Step 5.`\|`CPPOVR`| :small_orange_diamond:

You have to be very careful as sometimes you will not get the result you expect when you store fractoinal numbers.  `1.9` will get represented as `1.89999999999...`. 

So we have to be very careful with fractional numbers or errors may occur.

![imprecise](images/imprecise.png)

![](../images/line2.png)

##### `Step 6.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond:

In algebra you might remember that `(A + B) * C` is the same as `(A * C) + (B * C)`. So with integers this will be true.  Try doing this below. We get the exact same result as we expected.

![factoring out works](images/algebra1.png)

![](../images/line2.png)

##### `Step 7.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now if we do this ame thing with **double** values then we are not guaranteed to get the same result as each fractional number will be slightly different.  We also have to be careful about checking for sameness of to floating point numbers which again, cause bugs.

Finaly lets confirm that a double on our machine is **8 bytes**. On windows 11, with a 64 bit processor it is.

![error in factoring out doubles](images/doubleError.png)

![](../images/line2.png)

##### `Step 8.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:
A float literal is half the size of a double and is represnted by a decimal `.`, a fractional part if needed an finished with a lower case `f`.  So `13.45` is of type **double** and `13.45f` is of type float. As you can can see floats can're represent fractional numbers as accurately and have less precision than doubles. A float can only represent a number with 9 digitsfor the significand

![float type](images/floatType.png)

![](../images/line2.png)

##### `Step 9.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

A float is different from a double and we use the character `f` at the end of the number.  So `1.1` is a double and `1.1f` is a float.  Lets give it a shot:

![float type](images/floatPrint.png)

![](../images/line2.png)

##### `Step 10.`\|`CPPOVR`| :large_blue_diamond:

The size of a float is only 4 bytes (32 bits) so it cannot store as accurate a representation of the number and has greater error than a double.

![size of float](images/sizeOfFloat.png)

![](../images/line2.png)

##### `Step 11.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: 

One thing we have to be very careful about is that even a variable of type float has no effect on the literal on the right side of the `=` operator.  If we divide two **integers** we will get an interger set to the float.  So `9/2` does not return `4.5`.

![division with ints](images/carefulFloatDiv.png)

![](../images/line2.png)

##### `Step 12.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

It only takes one of the `literals` to be of type **float** and then the result will be fractional.

![fractional division of floats](images/floatFractions.png)

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Bools and Unsigned Ints"> -->

![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../operators/README.md#user-content-arithmetic-operators)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../bools/README.md#user-content-primitive-data-types---bools-and-unsigned-ints)|
|---|---|---|
