# Getting Started With D
> This is a work-in-progress reference for new users to get started with using D in their respective area of interest. Please make a pull request if you have something to contribute.

This a reference guide on **Getting Started with D**. Not everything will be written by me since I'm aware there's several existing resources...more of creating an entry point to all those resources (and writing more only when necessary). This is meant to be an up-to-date guide.

> It's difficult to find any resources on D outside its own documentation, which can make it a bit more challenging to get into - especially if you're quite new to programming.

I'm looking to cover areas such as:

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

## [ ] [General Overview](#)
The D programming language general purpose programming language that compiles to native code. You'll find D to be familiar but modern language with a simple C-like syntax. For these reasons D makes for a good language choice for both performance code and application development.

[snippet] Walter, Andrei and the D community work to make D a practical language that combines native code efficiency and control with the modeling power, safety, and productivity found in high-level languages and those that stick strictly to a single paradigm. If you enjoy languages D is interesting in the way it combines many paradigms in a C-like syntax, and yet D is also a language used in production at scale in industry and academe. 

If you've never used D before "Modeling Power" may not make much sense to you, but after you've used D you'll understand precisely what it means.  D is definitely fun to program in. 

I think where D really excels is with the combination of Phobos and the C/C++ bindings. The greatly-reduced number of functions I was writing was wonderful as D seemed to have everything. Combine that with some really good cross-compatibility with what are essentially the two biggest languages is the cherry on top. D can do anything C or C++ can do, only with greater ease.

The key with D is that it's not really supposed to be another lower-level language in the region of C++. It's much higher-level than that, but at the same time doesn't go as far up as your dotnet and jvm stuff to the point of bloat and sluggishness. It hits a sweet spot in the middle of easy use and great performance. It's not the best at either, but it's definitely good at both.

> [Many] of D's improvements appear to be small, but the aggregate is large enough that once you write a project
in D, you'll find it pretty hard to go back to another language - **Walter Bright, Creator of D**

> D has moved well ahead of
any other language in its abilities to support and integrate multiple paradigms like imperative, OOP, and
generic programming. - **Walter Bright, Creator of D**

> D used to have a slogan with 3 pillars: Modeling power, modern convenience, and native efficiency. 

[ref](https://wiki.dlang.org/Why_program_in_D)

## [ ] [Develpment tools and resources](#)

## [WIP] [Game development](/games.md)

Resources for game developers
[YouTube channel by Ki Rill](https://www.youtube.com/playlist?list=PLgM-lc_kSqFQPF0UXgmFZpZalqcrSofe-) on beginner game development

>  I'm talking about using the GC, but using it strategically. There are a number of ways to reduce pressure on the GC and minimize its impact on without dropping the benefits you get from the standard library, the runtime, and the GC itself. And they aren't onerous. Really, most of the people I see reaching first for betterC are throwing the baby out with the bathwater. There's no reason for it most of the time.

> D is not a managed language. The GC will only ever run a collection during an allocation, so you use the same strategy for allocation as you do in a C or C++ game engine: preallocate as much as possible, avoid allocations in your loops. See https://dlang.org/blog/the-gc-series/.

> According to success of Unity and my experience working with it having GC is actually great for game development but it is a no go for many core engine functionalities.

> Both the UE4 and Unity game engines use GC. Additionally, AAA games built with UE4 have shipped on consoles. UE4's GC certainly has issues (among other things), but you can still ship a game with it.

## [ ] [Writing scripts](#)

Since D provides type inference, high-level constructs, and fast compile-time it is a great language for writing scripts. The first line of the file is ignored if it begins with #! ('shebang') and combining this with rdmd which handles dependency resolution, D becomes a leader in native-code scripting languages.

```d
 #!/usr/bin/env rdmd
void main() {
    import std.stdio : writeln;
    writeln("Hello, World!");
}
```

## [ ] [Desktops Development](#)
Each language has a preferred application domain. D has a high degree of versatility as a language - it does have a sweet spot in high performance desktop and server side applications, but it can nonetheless be used where a scripting language would be the traditional choice: it provides the performance of low-level languages (of the order of C++) with the safety and ease of expression reminiscent of languages like Java and Python.

In fact, nearly everywhere Java is suitable, D could replace it, bringing in more expressive power, better performance and better memory management. Although its current libraries are nowhere near as extensive as the Java libraries, most fundamental bricks are already here, and D has native interfacing to both C and C++, with library solutions for other languages such as Python,R and Lua. You may want to have a look at Phobos and Deimos libraries, as well as third-party libraries to make your own opinion on that matter. A very nice port of Java's SWT library has been created under the name DWT (with older but more complete documentation available at the legacy dsource site). There are also bindings for GTK, and a cross-platform idiomatic D GUI. 

## [ ] [Embedded programming](#)

Being targeted at 32 bit and 64 bit machines, D is not designed for embedded development on small devices. However, with the advent of Android and iOS smartphones which embed powerful CPUs and large amounts of RAM, D may be suitable for such development. The GCC and LLVM compiler backends being able to target these devices, the community is making progress.

[ref](https://stackoverflow.com/questions/1207958/getting-embedded-with-d-the-programming-language)

