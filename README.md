

# Project Outline

I am making a chat app with raylib, on the web.
I am using a proccess to get c and its standard libraies to compile to webasm without emscripten.
The server backend will implement http1.1 and be written in c aswell. 
For c to wasm, I am going to be using a process outlined by this 
webpage.

webpage :
https://depth-first.com/articles/2019/10/16/compiling-c-to-webassembly-and-running-it-without-emscripten/

the general outline is as follows
* use a llvm installation and clang to compiler c to wasm.
* use the wasi-defined libc / replace libc with wasi-libc in llvm.
* fill in missing files (precompiled wasm binary).
* specific in the commincation between c, javascript, and webasm.


## some goals
* implement full secerity checks for webserver
