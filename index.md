I'm a Computer Science MSci student at the University of Birmingham (graduating in June 2020) and I have an interest in CPU architecture, compilers and operating system development. Check out some of my projects below.

# Projects

## [Pluto](https://github.com/SamTebbs33/pluto)
I am writing a kernel in [Zig](https://ziglang.org) that targets x86. I will begin work on x86-64, arm and aarch64 backends some time in the future.

It aims to be built entirely from scratch (it will have its own text editor, shell and perhaps even version control system) except for the compiler, which will be a ported version of Zig.

![Pluto welcome screen](https://github.com/SamTebbs33/pluto/raw/develop/hello.jpg)

## [Fero CPU](https://github.com/SamTebbs33/fero-cpu)
I am designing and implementing an embedded CPU architecture using verilog. The aim is to design an architecture with hardware support for multitasking.

# Awesome things

## [Zig](https://ziglang.org)
Zig is an up and coming systems programming language that aims to compete with C. It was created by [andrewrk](https://github.com/andrewrk) and some of my favourite features include:

* **Cross-compilation**: Every build of the compiler supports every backend so you don't have to build a version specific to a certain architecture, and compiling for another platform is as simple as setting the *-target* flag.
* **Error handling made easy**: It's possible to return an error or a valid value, meaning you don't have to return awkward integer values when something goes wrong in your function. Errors can be defined, thrown, caught and handled simply and without pain.
* **Memory management**: Any part of the standard library that you don't pass a memory allocator to will never allocate any memory. This means that you can specialse your memory management policy to your application and that the standard library can be used in freestanding mode.
* **Optionals**: No more just-in-case null checking if you specify that something cannot be null. Unwrapping a possibly-null value is fully safety checked and made straightforward.
* **No undefined behaviour**: Any operation that would introduce undefined behaviour in C is safety checked, meaning it will be caught and reported at runtime. This can be disabled using the *release-small* or *release-fast* build modes.
* **Compile-time code execution**: Zig code can be run at compile-time, completely mitigating the need for a preprocessor. A great writeup about this is [here](https://kristoff.it/blog/what-is-zig-comptime/).
* **It is its own build system**: It provided a flexbile build system baked directly into the compiler, meaning you can write build scripts in Zig and use them to build your application.
* **Total C interoperability**: Zig can interoperate with C code with no messy bindings. It is also a C compiler!
