UWindsor COMP-3520 SDL2 Project Template
===

Floordemo branch
---

This branch contains source code for some 2.5D rendering functions written
for software rendering.  The code needs a bit of cleaning up, but otherwise
should work fine.  Pull requests are welcome to improve the code.
It will be kept in parity with the `floordemo` branch in SDL2TemplateCMake.

The code is written in mostly C such that students without a C++ background
can more easily understand it.  There are some parts that need to be overhauled,
like the conversion from floating point coordinates to integer coordinates.
However, the basic ideas should be evident.  In class, we'll discuss how
this would have been implemented using fixed-point arithmetic.

A live demo compiled using Emscripten and WebAssembly is available [here](https://inbetweennames.github.io/SDL2TemplateCMake/)

Introduction
---

This template is intended for students in the COMP-3520 Introduction to Computer Graphics course
at the University of Windsor, however it should serve as a useful template for anyone interested in
getting started with the [SDL2](http://libsdl.org/) library quickly on Windows using Visual Studio.
It defaults to 64-bit executables with static linking only, which is ideal for learning purposes.

The following header files and precompiled static libraries are included:
* [SDL2](http://libsdl.org/) 
* [SDL2_ttf](https://www.libsdl.org/projects/SDL_ttf/) library for easy text rendering
* [freetype2](https://www.freetype.org/) which `SDL2_ttf` uses for the actual work

Only Visual Studio 2017 with the `v141` toolchain is supported at this time.
If this is a problem, just let me know by either creating an issue or sending me an email.

Linux, Mac, Cygwin, MSYS2, Git-for-Windows SDK users
---

See my other repository for a CMake version of this repository that uses dynamic linking instead:
[SDL2TemplateCMake](https://github.com/InBetweenNames/SDL2TemplateCMake)

Windows users
---

This template allows you to get started right away after installing Visual Studio 2017.
Simply `git clone` this template onto your system, and open `SDL2Template.sln` in Visual Studio.
Next, build it and run the sample program.
You can use this as your starting point for all coursework.

Note that I don't require you to use Visual Studio 2017 for the course -- if you want to use Cygwin or MSYS2,
you certainly can.  The instructions should be similar to what is in the `Linux users` section.

The demo
---

The sample code provided should display "Hello World!" in a window on your screen when run.
You can clone this project as many times as you need for different assignments.

Recommended practices
---

Students who know C++ are encouraged to use it, however, C++ is not a requirement for the course.
The sample code provided is mostly C compatible for the benefit of students who haven't had much C++ exposure yet.

Static Code Analysis is enabled by default on Debug builds.  If you see compiler warnings in your code,
don't ignore them!

When we get to the more mathy parts of the course, if you have a good handle on C++, consider using
[Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page) for your Linear Algebra needs.

Extra goodies:
---

Although this template has everything you need to succeed in the course, in your own personal projects
it's likely you'll want to go even further.  Consider adding the following libraries for your arsenal:

* [SDL2_image](https://www.libsdl.org/projects/SDL_image/) for easy image loading from a variety of formats
* [SDL2_net](https://www.libsdl.org/projects/SDL_net/) for a basic cross-platform networking library
* [SDL2_mixer](https://www.libsdl.org/projects/SDL_mixer/) for sound rendering
* [SDL2_rtf](https://www.libsdl.org/projects/SDL_rtf/) for basic document handling (RTF)

Bugs:
---

If you find any problems with the template, please let me know by either creating an Issue on the project page or sending
me an email.
