# Getting Started With D
> This is a work-in-progress reference for new users to get started with using D in their respective area of interest. Please make a pull request if you have something to contribute.

This a reference guide on **Getting Started with D**. Not everything will be written by me since I'm aware there's several existing resources...more of creating an entry point to all those resources (and writing more only when necessary). This is meant to be an up-to-date guide.  I'm looking to cover areas such as:

* Leaning resources.
* Development tools available in D Window, Linux, Mac
* Setting up a development environment
* Resources from web/server-side developers
* Resources for game and graphics developers
* Resources for scientific computing
* Resources for desktops development (system, GUIs, ...??)
* Resources for data science (taken separately from general scientific computation)
* Resources for embedded programming
* How and where to get help
* D community platforms (forum, IRC, ???)
* How to contribute to D open source and tools (referencing existing efforts and progress)

> Let me know what else I'm missing

I started this as a [post in the D forums to collect some community feedback](https://forum.dlang.org/post/itxvymhjgmfqdihnswly@forum.dlang.org). If you have something to share or a resource you think I should add, please don't hessitate to **create an issue here** or **post in the forum thread*** reference above. Pull requests are also welcomed, cheers!

## [ ] [General Overview]()
The D programming language general purpose programming language that compiles to native code. You'll find D to be familiar but modern language with a simple C-like syntax. For these reasons D makes for a good language choice for both performance code and application development.

> [Many] of D's improvements appear to be small, but the aggregate is large enough that once you write a project
in D, you'll find it pretty hard to go back to another language - **Walter Bright, Creator of D**

> D has moved well ahead of
any other language in its abilities to support and integrate multiple paradigms like imperative, OOP, and
generic programming. - **Walter Bright, Creator of D**

D has a high degree of versatility as a language - it does have a sweet spot in high performance desktop and server side applications, but it can nonetheless be used where a scripting language would be the traditional choice: it provides the performance of low-level languages (of the order of C++) with the safety and ease of expression reminiscent of languages like Java and Python. 

[ref](https://wiki.dlang.org/Why_program_in_D)

## [ ] [Develpment tools and resources]()

## [WIP] [Game Development](/games.md)
Resources for game developers

## [ ] [Desktops Development]()
In fact, nearly everywhere Java is suitable, D could replace it, bringing in more expressive power, better performance and better memory management. Although its current libraries are nowhere near as extensive as the Java libraries, most fundamental bricks are already here, and D has native interfacing to both C and C++, with library solutions for other languages such as Python,R and Lua. You may want to have a look at Phobos and Deimos libraries, as well as third-party libraries to make your own opinion on that matter. A very nice port of Java's SWT library has been created under the name DWT (with older but more complete documentation available at the legacy dsource site). There are also bindings for GTK, and a cross-platform idiomatic D GUI. 
