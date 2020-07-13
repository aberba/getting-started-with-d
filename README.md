# Getting Started With D

This is a beginner friendly guide for new users to get started with using [D programming language](https://dlang.org) in their respective areas of interest. It's an opinionated and up-to-date entry point into the D ecosystem with focus on the most important information needed to get started. Other resources are also referenced when necessary.

> It's difficult to find any resources on D outside its own documentation, which can make it a bit more challenging to get into - especially if you're quite new to programming ― **Anonymous user**

I'm looking to cover areas such as:

- Leaning resources.
- Development tools available in D Window, Linux, Mac
- Setting up a development environment
- Resources from web/server-side developers
- Resources for game and graphics developers
- Resources for scientific computing
- Resources for desktops development (system, GUIs, ...??)
- Resources for data science (taken separately from general scientific computation)
- Resources for embedded programming
- How and where to get help
- D community platforms (forum, IRC, ???)
- How to contribute to D open source and tools (referencing existing efforts and progress)

I started this with [a post in the D forums to collect some community feedback](https://forum.dlang.org/post/itxvymhjgmfqdihnswly@forum.dlang.org). If you have something to share or a resource you think I should add, please don't hesitate to **create an issue here** or **post in the forum thread** reference above. Pull requests are also welcomed, cheers!

## General Overview

D is a general purpose system programming language that compiles to native code. You'll find D to be a familiar modern language with a simple and clean C-like syntax. For these reasons D makes for a good language choice for both performance code and application development.

```d
// sample clean D code
import std.stdio;

void main(){
    writeln("Hello world");
}
```

Walter Bright (the creator), Andrei Alexandrescu (co-creator) and the D community work hard to make D a **practical language** that combines **efficiency and control** with the **modeling power, safety, and productivity** you would expect from a modern high-level languages. D is particularly interesting in the way it combines many styles of programming. Its no surprise D is used in production at scale in [industry and academia](https://dlang.org/orgs-using-d.html).

> If you've never used D before "Modeling Power" may not make much sense to you, but after you've used D you'll understand precisely what it means. D is definitely fun to program in. ― **Anonymous user**

> Many of D's improvements appear to be small, but the aggregate is large enough that once you write a project
> in D, you'll find it pretty hard to go back to another language ― **Walter Bright, Creator of D**

> I think where D really excels is with the combination of Phobos [, the standard library] and the [interface with other languages]. The greatly-reduced number of functions I was writing was wonderful as D seemed to have everything. Combine that with some really good cross-compatibility ... is the cherry on top. D can do anything [other languages] can do, only with greater ease. ― **Anonymous user**

> The key with D is that it's not really supposed to be another lower-level language ... It's much higher-level than that, but at the same time doesn't go as far up ... to the point of bloat and sluggishness. It hits a sweet spot in the middle of easy use and great performance. It's not the best at either, but it's definitely good at both. ― **Anonymous user**

> D has moved well ahead of
> any other language in its abilities to support and integrate multiple paradigms like imperative, OOP, and
> generic programming. - **Walter Bright, Creator of D**

[ref](https://wiki.dlang.org/Why_program_in_D)

## [Development Tools](#)

...

## Application Development

...

[Learn more...](/apps.md)

## Scripts and Automation

Since D provides type inference, high-level constructs, and fast compile-time it is a great language for writing scripts. The first line of the file is ignored if it begins with #! ('shebang') and combining this with rdmd which handles dependency resolution, D becomes a leader in native-code scripting languages.

```d
 #!/usr/bin/env rdmd
void main() {
    import std.stdio : writeln;
    writeln("Hello, World!");
}
```

[Learn more...](#)

## [Embedded Systems Programming](#)

Being targeted at 32 bit and 64 bit machines, D is not designed for embedded development on small devices. However, with the advent of Android and iOS smartphones which embed powerful CPUs and large amounts of RAM, D may be suitable for such development. The GCC and LLVM compiler backends being able to target these devices, the community is making progress.

[ref](https://stackoverflow.com/questions/1207958/getting-embedded-with-d-the-programming-language)

[Learn more...](#)
