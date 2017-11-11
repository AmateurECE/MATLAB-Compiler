# An Open Source MATLAB Toolchain #

This repository will contain a minimal, yet fully-functional, open-source MATLAB
toolchain, including a compiler, which will convert most standard MATLAB source
code programs to target machine code, and also a standard library, which will
implement most of the MATLAB standard library in Fortran95 and pure C. As such,
the requirements for installation will be:

* A fully functional C compiler, such as GCC.
* A fully functional Fortran95 compiler, such as gfortran (included in the
  GCC package).

Obviously, this repository is not complete. It will follow the workflow
described herein:

- [ ] Derive a complete BNF Grammar for the MATLAB Language
- [ ] Implement a lexical parser for the language
- [ ] Implement a semantic analyzer for the language
- [ ] Implement an intermediate language compiler
- [ ] Include minimal code optimization routines
- [ ] Generate assembly for the target architecture
- [ ] Convert this assembly to target machine executable code

These steps may be completed in any order. The compiler will not support
debugging, nor will it include facilities to generate debugging symbols for
the target machine. Code optimization will be supported in a most minimal
manner, and target-specific optimizations may not be supported at all. The
purpose of this project is to implement a simple, fast compiler, which will
successfully compile most syntactically correct MATLAB programs, and will
hold the programmer fully responsible for his/her coding practices. This README
will be updated as work is completed on the project.
