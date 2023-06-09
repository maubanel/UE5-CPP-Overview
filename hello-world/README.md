![](../images/line3.png)

### Hello World

Print hello world to the console of visual studio.

[home](../README.md#user-content-ue5-cpp-overview) • [next](../errors/README.md#user-content-errors)</sub>

![](../images/line3.png)

Chapter introduction here.

<br>

---

##### `Step 1.`\|`CPPOVR`|:small_blue_diamond:

## Why C++

Out of all the modern programming languages why do we still use C++ for games?

* *Performance*. C++ is a high-performance lower level programing languag.  Games are very performance oriented and c++ allows user to use computer hardware efficiently.  Often higher level scripting languages are used for game play scripting. [Unity](https://answers.unity.com/questions/9675/is-unity-engine-written-in-monoc-or-c.html) game engine is written in c++ but you write all the game scripts in c#.

* *Compiles*. C++ is a compiled programming language.

* *Low Level*. C++ gives developers low-level access to the computer hardware, allowing them greater control and optimize harware usage. It is used extensively in lower level systems like rendering, audio and physics

* *Memory Management*. Manual memory management which avoids any issues with higher level languages not freeing up memory, or freeing up so much that it affects the performance of the game.

* *Optimizable*. Easier to optimize heavily used routines

* *Portability*. There is a C++ compiler available for all platforms, so is beneficial if you want to support PC's, consoles and mobile.

* *Language features*.  C++ had advanced features such as templates, memory management and object-oriented programming.

* *Existing libraries*. Many libaries such as Havok or Scaleform are written in C++.

* *CPP 17*. We will be using C++ 17 as this is supported by Unreal.

* *Industry standard*. C++ is one of the most widely used programming languages in the game industry, so developers can benefit from a large community of resources, libraries, and tools to create their games.

> Modern C++ Language Syntax
Unreal Engine is built to be massively portable to many C++ compilers, so we are careful to use features that are compatible with the compilers we might be supporting. Sometimes features are so useful that we will wrap them up in macros and use them pervasively. However, we usually wait until all of the compilers we might be supporting are up to the latest standard.<br/><br/>Unreal Engine requires a minimum language version of C++17 to build, and we use many modern language features that are well-supported across modern compilers. In some cases, we can wrap up usage of these features in preprocessor conditionals. However, sometimes we decide to avoid certain language features entirely, for portability or other reasons.<br/><br/>Unless specified below, as a modern C++ compiler feature we are supporting, you should not use compiler-specific language features unless they are wrapped in preprocessor macros or conditionals and used sparingly. - [UE5 Documentation](https://docs.unrealengine.com/5.0/en-US/epic-cplusplus-coding-standard-for-unreal-engine/#modernc++languagesyntax)

![](../images/line2.png)

##### `Step 2.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: 

Install [Visual Studio 22 (Community will work)](https://visualstudio.microsoft.com/downloads/) and include the libraries that we will need which includes the **Game development with c++** as well as the **Unreal Engine installer**, **C++ profiling tools**, **C++Address Sanitizer**, **Windows 10 SDK** (10.0.18362 or newer).  Their screenshot also says to include the **.NET desktop-development** as well as the **Universal WIndows Platform development**. Feel free to follow the rest of the recommended settings in the [Setting Up Visual Studio](https://docs.unrealengine.com/5.2/en-US/setting-up-visual-studio-development-environment-for-cplusplus-projects-in-unreal-engine/) or when we use it with Unreal Engine.

![install required components into vs 22](images/vs-install-workloads.jpg)


![](../images/line2.png)

##### `Step 3.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up the newly configured **Visual Studio 2022**. You should see a window to create a new project.  Click on the **Create a New Project** button:

![Screenshot of Microsoft's Visual Studio Community create project page](images/CreateNewProjectVS22.png)

![](../images/line2.png)

##### `Step 4.`\|`CPPOVR`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Select a C++ **Console App** as we will only be working within the console. Meks sure it is a C++ console app as there are many programming languages that Visual Studio supports out of the box.  Press the <kbd>Next</kbd> button.

![select c++ console app](images/SelectConsoleApp.png)

![](../images/line2.png)

##### `Step 5.`\|`CPPOVR`| :small_orange_diamond:

Name the project and select a location to save it in and press the <kbd>Create</kbd> button.

![name cpp project and set directory](images/NameTheFile.png)


![](../images/line2.png)

##### `Step 6.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond:

Now Visual Studio defaults to C++ 14 so lets change it to C++ 17.  Go to **Project | CPPOverview Properties** and open up **C/C++** and select **Language**.  Double click the language until you get to **ISO C++17 Standard**.  Press the <kbd>Apply</kbd> then <kbd>OK</kbd> buttons.

![change to cpp 17](images/setCPP17.png)


![](../images/line2.png)

##### `Step 7.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

You should get a stubbed in project that prints "Hello World" to console.  First lets look at the elements.  We include the `<iostream>` libraries.  This includes the global object `std::cout` that controls the output stream buffer.  This allows us to access the stream that eventually gets sent to the console. <br><br>`std` is the namespace that represents the word \'standard\' which are built in **C++** libraries available on all platforms including **Windows** which we are working on now.<br><br>`"Hello World\n"` is a string with a new line (`\n`) which gets stored as a single character.<br><br>All lines that begin with `//` are comments and are not compiled into the final project.  These are here for you to read and explain to yourself and other developers the intent of what you are trying to do.

![A screenshot of the default www.onlinegdb.com webpage with C++14 selected](images/SelectCPPLanguage.jpg)

![](../images/line2.png)

##### `Step 8.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now clean up the comments inside the `main` brackets ({}) (everything with a `//` before it).  Now run the game by selecting the run button with `Local Windows Debugger` selected or just press the `F5` button.

![Running the default www.onlinegdb.com webpage with C++14 selected](images/HelloWorld.jpg)

![](../images/line2.png)

##### `Step 9.`\|`CPPOVR`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

So the end result is in the console should look something like:

![remove comments and run](images/Comments.png)

![](../images/line2.png)

##### `Step 10.`\|`CPPOVR`| :large_blue_diamond:

C is completely compatible inside of C++.  So we can also print using the older C style format which is used extensively in Unreal.

There are always more than one way to skin a cat, so we can also call a function called `printf` and pass it the "Hello World" string as a parameter. Run it by pressing the green run button or `F5` and notice that it should have the same end result. Notice that this is in global name space and we did not need to include `std::`.

![Highlights the included file <stdio.h> in c++14](images/IncludeStdioh.png)

![](../images/line2.png)

##### `Step 11.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: 

Click on the [cplusplus.com printf reference](http://www.cplusplus.com/reference/cstdio/printf/). Notice that it includes a **function** called `printf` (we will explain functions in a future lesson). Without libraries and built in functions, the language is fairly limited.  Anytime we need to do anything specialized for a specific OS and system, we probably need to load a set of libraries.

![Screenshot of cplusplus.com's definition of the printf function](images/printfDescription.png)

![](../images/line2.png)

##### `Step 12.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Every C++ program starts by calling a function called **main**.  We know if is a function as it is a name followed by **()** parenthesis.  It then runs everything between the following curly braces `{....}`. It executes them in order line by line, in my case it only runs line 8.

![Highlights the main(){...} function in a C++14 program](images/RunMain.png)

![](../images/line2.png)

##### `Step 13.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

So the first thing the program does in **main()** is to run the function `printf` and passes a string parameter of **"Hello World"**. We will get into this more shortly when we dive into strings.

![Highlights the printf function in a C++14 program](images/printfFunction.png)

![](../images/line2.png)

##### `Step 14.`\|`CPPOVR`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

What this line does is print the string passed to it to the console.  In this case it prints **Hello World**.

![Shows console output of Hello World in C++14 console output](images/hw2.png)

![](../images/line2.png)

##### `Step 15.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond: 

When you press run the program is compiled.  What does this mean?  This is the process of going from a human readable form script and creates object code that forms an executable (an .exe on a PC).  So the compiler turns it from words into zeros and ones (machine code).

![Illustration of a program that goes from a source file to machine code](https://www.thecrazyprogrammer.com/wp-content/uploads/2018/05/Difference-between-Source-Code-and-Object-Code.png")

![](../images/line2.png)

##### `Step 16.`\|`CPPOVR`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

It is customary to add `return 0` to the end but should work without it on most platforms.  This function returns to its caller (we don't call it) a 0.  So if the program runs and doesn't crash it should finish with an exit code of 0. Look at the second line of the **Debug Console** window and you will see `exited with code 0`.  This means the program completed without crashing.

![Highlights return 0 in C++14 program](images/Return0.png)

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Errors"> -->

![next up - ](images/banner.png)

![](../images/line.png)

| [home](../README.md#user-content-ue5-cpp-overview) | [next](../errors/README.md#user-content-errors)|
|---|---|
