# Welcome to OpenCilk

This beta version is meant for experienced Cilk users running
Unix/Linux on modern x86_64 processors (e.g., Haswell, Excavator,
or newer).  This version has been tested on Ubuntu 18.04, FreeBSD 12.1,
Fedora 30, and Mac OS X 10.15.

Here is a summary of features in this version of OpenCilk:
* The `cilk_spawn`, `cilk_sync`, and `cilk_for` keywords are enabled by using
  the `-fopencilk` command-line argument and including `<cilk/cilk.h>`.
* The compiler is based on LLVM 9 and supports the usual clang options.
* Both C and C++ are supported.
* Prototype support for C++ exceptions is included.
* Reducer hyperobjects are supported using the Intel Cilk Plus
  reducer library -- i.e., the hyperobject headers from Intel Cilk Plus 
  -- except that it is not valid to reference the view of a C reducer
  after calling CILK_C_UNREGISTER_REDUCER.

## Install
[Instructions](https://github.com/OpenCilk/infrastructure/blob/release/INSTALLING.md) for building OpenCilk **from source**.


## Docker
[Scripts](https://github.com/OpenCilk/infrastructure/blob/release/docker) for building a Docker image with OpenCilk.
  

## Examples
Some simple [demo Cilk programs](https://github.com/OpenCilk/tutorial).

[Additional demo](https://github.com/OpenCilk/applications) Cilk programs.

---

Bug reports should be emailed to bugs<em>[at]</em>opencilk.org.  Other queries and
comments should be emailed to contact<em>[at]</em>opencilk.org.

The OpenCilk development team:\
Tao B. Schardl, MIT - Director, Chief Architect\
I-Ting Angelina Lee, WUSTL - Director, Runtime Architect\
John F. Carr, consultant - Senior Programmer\
Dorothy Curtis, MIT - Project Manager\
Charles E. Leiserson, MIT - Executive Director\
Alexandros-Stavros Iliopoulos, postdoc, MIT\
Grace Q. Yin, intern, MIT
