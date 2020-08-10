# ToyLisp: A Simple Lisp Implementation in C - WASM Implementation #

This is a working example of a working WASM Implementation of LISP based on Kim, Taegyoons work.

Steps:
1. Install webassembly (from here: https://webassembly.org/getting-started/developers-guide/):
```
$ git clone https://github.com/emscripten-core/emsdk.git
$ cd emsdk
$ ./emsdk install latest
$ ./emsdk activate latest
```
2. git clone git@github.com:michaelachrisco/ToyLisp.git
3. `cd ToyLisp`
4. `emcc ToyLisp.c -s WASM=1 -o toy.html`
5. `python -m SimpleHTTPServer 8000` or `python3 -m http.server`
6. go to your browser and navidate to toy.html A prompt should pop up. Type in some LISP code and it should work in place.
`Suggested (+ 1 1)`

(C) 2014 Kim, Taegyoon

Based on Leo Howell's [Building LISP](http://www.lwh.jp/lisp/index.html) with bug fixes and enhancements.

Case-sensitive Lisp-1

Enhancements:

* Built-in symbol comparison
* Windows support
* Multiple expressions in the REPL
* C++ compliance

## License ##

   Copyright 2014 Kim, Taegyoon

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

   [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
