![](../images/line3.png)

### Order of Operations

<sub>[previous](../init/README.md#user-content-initialization) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../selection/README.md#user-content-selection-and-iteration)</sub>

![](../images/line3.png)

The C++ compiler will perform mathematical operations in the [correct order](https://en.cppreference.com/w/cpp/language/operator_precedence).  Look at the link to get a full description of what order of operations C++ uses on non-mathematical operations.

Operator precedence: C++ follows the standard mathematical operator precedence rules, such as multiplication and division being evaluated before addition and subtraction. However, if you have a complex expression with multiple operators, it's important to use parentheses to clarify the intended order of operations.
<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

Right click on the solution and select **Add | New Project...** then select a C++ **Console Application**. Call the new project `OrderOfOperations` and press the <kbd>Create</kbd> button.

![alt_text](images/addOrderOfOpsProject.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

*Right click* on **OrderOfOps** project and select **Properties** and and change the C++ Language to `C++ 17`.

![add OrderOfOps.cpp to source folder](images/orderOfOpsCpp.png)

![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

*Right click* on **OrderOfOperations** project and select **Run 'OrderOfOperations'** so this is the one that runs with it's `main(){}` function.

![alt_text](images/setAsStartup.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Add a comment at the top of the project and include <iostream> and add a `main(){}` function.  Then we will do the following arithmetic: `12 + 13 * 2`.  So C++ will follow mathematical order of operations and will multiply `13 * 2` first then add `12` which will give us a answer of `38`.

![order of operations followed fro 12+13*2](images/standardOrderOfOps.png)

![](../images/line2.png)

##### `Step 5.`\|`CPPOVR`| :small_orange_diamond:

Even though the brackets are not  necessary, I typically include them in my code so that it is crystal clear that I know how I want it to resolve to be extra verbose/obvious.

In mathematics and programming, parentheses are used to indicate the grouping of operations and specify the order of evaluation. When an expression contains multiple sets of parentheses, the innermost parentheses are evaluated first, followed by the outer ones. This concept is known as the "order of operations" or "operator precedence."

The order of operations is typically represented by the acronym PEMDAS (or BODMAS), which stands for:

1. Parentheses: Operations within parentheses are evaluated first. Any expression enclosed in parentheses is treated as a separate unit and takes precedence over other operations.

2. Exponents (or Powers): After evaluating parentheses, exponents are calculated. Exponentiation involves raising a number to a power. For example, in the expression `2^3`, the exponentiation operation raises 2 to the power of 3, resulting in 8.

3. Multiplication and Division: After evaluating parentheses and exponents, multiplication and division operations are performed from left to right. These operations are given equal precedence, so they are evaluated in the order they appear in the expression.

4. Addition and Subtraction: Lastly, addition and subtraction operations are performed from left to right. Like multiplication and division, these operations have equal precedence and are evaluated in the order they appear.

It's important to note that parentheses can be nested, meaning that there can be multiple levels of parentheses within an expression. In such cases, the innermost set of parentheses is evaluated first, followed by the outer sets, moving outward until the entire expression is evaluated.

Here's an example to illustrate the order of operations using parentheses:

Expression: `(12 + 13) * 2`

1. Evaluate the innermost set of parentheses: `(12 + 13)` equals `25`.
2. Perform multiplication: `25 * 2` equals `50`.

By using parentheses to explicitly group operations, you can control the order in which they are evaluated, ensuring that your expressions are calculated correctly according to the intended logic. It is sometimes good to include parenthesis such as 12 + (13 * 2) even if not necessary to be very explicit about what you are doing.

![changing order of operations](images/followBrackets.png)

![](../images/line2.png)

##### `Step 6.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond:

We have to be careful when using expressions as there are no standard mathematical rules for them.  When using expressions you may not get what you think.  So `++I * 2` when I is equal to `12` is not the equivalent of `I + 1 * 2` (which would be 24) but it resolves it as (I + 1) * 12 even though not expressed that way.  We get a result of `26`. 

![be careful when using expression](images/carefulBe.png)

![](../images/line2.png)

##### `Step 7.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Subtract `1` from `I` to get it back to `12`.  Then on the next line perform `I++ * 2`.  Now since the `++` operator will run after the statement, this will be interpreted as `12 * 2`.  The variable `I` will be incremented after the statement. On the next line `I * 2` becomes `13 * 2` which resolves to `26`.

![alt_text](images/moreBeware.png)

![](../images/line2.png)

##### `Step 8.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Modulo resolves just like multiplication and division - so before subtraction and addition. So `12 % 5 + 2 * 5` is solved thusly:

1. The compiler first solves `12 % 5` (2 remainder 2) with a value of `2`.
2.  Next it multipiles `2 * 5` for a result of `10`.
3.  Finally it adds `2 + 10` for an answer of `12`.  

Try it for yourself.

![12 % 5 + 2 * 5 = 12](images/moduloOrder.png)

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Selection and Iteration"> -->

![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../init/README.md#user-content-initialization)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../selection/README.md#user-content-selection-and-iteration)|
|---|---|---|
