![](../images/line3.png)

### Selection and Iteration

<sub>[previous](../order/README.md#user-content-order-of-operations) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../)</sub>

![](../images/line3.png)

In C++, there are selection and iteration operators that allow you to make decisions and repeat actions based on certain conditions. Here's a brief explanation of a selection of these operators:

**Selection Operators:**

* **if statement**: The if statement allows you to perform conditional execution of code. It evaluates a condition and executes a block of code if the condition is true. Optionally, you can include else and else if clauses to handle alternative conditions.

* pseudocode:
```cpp
if (ConditionIsTrue)
{
  //...Add logic to run if variable ConditionIsTrue is true
}
else if (anotherConditionIsTrue)
{
    //runs if first condition is false, can have as many else if's as we need
}
else
{
    // runs if all ifs and else ifs are false
}
```

* **switch statement**: The switch statement provides a way to select one of many code blocks to execute based on the value of a variable. It allows you to compare the variable against multiple cases and execute the code corresponding to the matching case. The switch statement also supports a default case for handling values that do not match any of the cases.

* pseudocode:
```cpp
switch(variable)
{
    case 1:
    // do something
    break;

    case 2: 
    // do something different
    break;

    default:
    // if none of the above cases apply always do the following
    break;
}
```

* **while loop**: The while loop repeatedly executes a block of code as long as a given condition remains true. It checks the condition before each iteration, and if the condition evaluates to true, the code block is executed. The loop continues until the condition becomes false.

* pseudocode:
```cpp
while(true)
{
    // do something
}
// the above will keep runing until the while statement changes to false

```

* **for loop**: The for loop allows you to repeatedly execute a block of code for a fixed number of iterations. It typically consists of an initialization statement, a condition for continuing the loop, an update statement, and the code to be executed in each iteration.

* pseudocode:
```cpp
for (startingpoint = some value; continue to run condition; increment startingpoint)
{
    // do something over and over until run condition above is false
}

```

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

Start a brand new **Empty Project** in C++ by *right clicking* on the solution in Visual Studio 19. Call it `SelectionIteration` and press the <kbd>Create</kbd> button.

![create SelectionIteration Project](images/selectionIterationProject.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

Right click on the **SelectionIteration** project and select **Set as Startup Project**.

![set as startup project](images/startUpProject.png)

![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Right click on the **Source** folder in the **SelectionIteration** project and right click and **Add | New Item...**.  Call it `SelectionIteration.cpp`.

![add selectioniteraction.cpp to source folder in project](images/addNewItem.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

In C++, comparison operators are used to compare two values or expressions and evaluate their relationship. These operators return a Boolean value (`true` or `false`) based on the result of the comparison. Here's a brief explanation of the common comparison operators in C++:

1. Equality Operator (`==`):
   - Checks if two values are equal.
   - Returns `true` if the values are equal, and `false` otherwise.
   - Note that unlike `=` an assignment operator, an equality `==` operator returns whether the left hand and right hand side operand are the same 
   
   Example:
   ```cpp
   int x = 5;
   int y = 7;
   bool result = (x == y);  // false
   ```

2. Inequality Operator (`!=`):
   - Checks if two values are not equal.
   - Returns `true` if the values are not equal, and `false` if they are equal.
   
   Example:
   ```cpp
   int X = 5;
   int Y = 7;
   bool result = X != Y;  // true
   ```

3. Greater Than Operator (`>`):
   - Checks if the left operand is greater than the right operand.
   - Returns `true` if the condition is true, and `false` otherwise.
   
   Example:
   ```cpp
   int X = 5;
   int Y = 7;
   bool result = (X > Y);  // false
   ```

4. Less Than Operator (`<`):
   - Checks if the left operand is less than the right operand.
   - Returns `true` if the condition is true, and `false` otherwise.
   
   Example:
   ```cpp
   int X = 5;
   int Y = 7;
   bool result = (X < Y);  // true
   ```

5. Greater Than or Equal To Operator (`>=`):
   - Checks if the left operand is greater than or equal to the right operand.
   - Returns `true` if the condition is true, and `false` otherwise.
   
   Example:
   ```cpp
   int X = 5;
   int Y = 7;
   bool result = (X >= Y);  // false
   ```

6. Less Than or Equal To Operator (`<=`):
   - Checks if the left operand is less than or equal to the right operand.
   - Returns `true` if the condition is true, and `false` otherwise.
   
   Example:
   ```cpp
   int X = 5;
   int Y = 7;
   bool result = (X <= Y);  // true
   ```
These comparison operators are used to make logical comparisons between variables, values, or expressions and help in decision-making within your program. The result of the comparison can be used in control structures like `if` statements and loops to determine the flow of execution based on specific conditions.

So in this **if statement** we are checking if `12 < 13`.  If this resolves to true (it will) then it will run all the code in the following curly braces.  Please note that this is not a statement so there is no `;` at the end of the `if`.  

![if statement](images/ifStatement.png)

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

| [previous](../order/README.md#user-content-order-of-operations)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../)|
|---|---|---|
