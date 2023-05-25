![](../images/line3.png)

### Errors

<sub>[previous](../hello-world/README.md#user-content-hello-world) • [home](../README.md#user-content-ue5-cpp-overview) • [next](../)</sub>

![](../images/line3.png)

Lets look at th emost common type of error.  When we mistype anything, it will usually create a syntax error and the program will not compile - thus not run. A syntax error is a grammatical error in the code that prevents the program from running. It mostly occurs when there is a mistake in the syntax such as missing a semicolon, using an incorrect keyword, or adding an extra closing bracket. These errors can be easily detected by the compiler and are shown as error messages that indicate the line of code that has the syntax error.

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

A visual studio solution can contain more than one project (a program with a main function). Lets create a new project by right clicking on the solution and select **Add | New Project...**.

![add project to solution](images/newProject.png)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

This time lets start the program from scratch, select a **C++ Empty Project**.  Press the <kbd>Next</kbd> button.

![add an empty c++ project](images/AddEmptyProject.png)

![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Right click on the **Source** folder in the new **Errors** project and select **Add | New Item...**.  Call the new file `errors.cpp`.  Press the <kbd>Add</kbd> button.

![add errors.cpp to source folder](images/addErrorscpp.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

In Unreal we will be using c style printing like we do here.  But lets go back to printing with `std::cout`. Lets look at the iostream libraries that includes 4 other libraries and gets us access to an **Object** called **std::cout** (standard output). We will be getting into objects later on. But we can call the **Object** `cout` and pipe it into an output stream.

![Screenshot of cppreference.com's difinition of standard library header \<iostream\>](images/iostreamdefinition.jpg)

We do this by adding the line `cout << "My name is Marc!";` replacing the call to the **printf()** function.  Press the **Run** button.  One of the thing the compiler does is sends an error intead of running the program. This means it did not compile and create a new executable.  In this case, it shows an error that cout is not in scope and is **undefined**.

![ighlight the line cout <<  &quot;My Name is Marc &quot; in a C++14 program"](images/FirstCout.jpg)

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 5.`\|`CPPOVR`| :small_orange_diamond:

Now lets add `std::` before the `cout` so that it will be in scope.  We will go into more detail later on describing this.  Press run and you should see it print the new message we typed. cout is an abbreviation for **character output stream**. Notice that we end the line with a `;` semicolon. Every line is a **statement** and has to be terminated by a semicolon. The compiler needs to know where one statement ends and the next begins.<br><br>Now the `<<` operator inserts the data that follows it into an [output stream](http://www.cplusplus.com/doc/tutorial/basic_io/) (which in our case will be the console displayed on the monitor).

![Create new sprite with button](images/stdcoutfix.jpg)

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 6.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond:

![alt_text](images/.png)

![](../images/line2.png)

##### `Step 7.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:
If we remove the semi-colon and try and run the program the compiler will give us an error when we press run (when we run it, the program is compiled and it tries to run it).  Try this and read the error.  Sometimes the error messages are clear and sometimes they are hard to read and understand. This is a compiler error.  In a script any spelling mistake or typing error will result in a program error of some sort.

![alt_text](images/NoSemicolonError.jpg)
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

| [previous](../hello-world/README.md#user-content-hello-world)| [home](../README.md#user-content-ue5-cpp-overview) | [next](../)|
|---|---|---|
