# Cuda Blitz
Imsar's Blitz++ alterations to allow for cuda managed memory allocation


Blitz with Cuda Allocation
==========================

Several changes have been made to blitz that allow it to allocate memory on the cpu, like normal, or in a shared memory state using cudaMallocManaged. This change was implemented for use with the Jetson board and is not tested with any other achitecture. Other minor changes have been implemented to remove errors and warnings that occured at compile time when `-std=c++11 -Wall` are used.
Also note that these changes have only been made to files used in our project. There may be warnings, compile errors, or runtime errors caused by these changes in other files. Please use caution if using this code.
Starting version of blitz++ was version 0.9

### Files Changed:
* blitz/array-impl.h
* blitz/array/eval.cc
* blitz/array/fastiter.h
* blitz/array/iter.h
* blitz/array/methods.cc
* blitz/array/resize.cc
* blitz/memblock.cc
* blitz/memblock.h
* blitz/range.h
* blitz/tinymat.h
* blitz/tinyvec.h
* blitz/vector.cc
* blitz/vector.h

See comments added to each of these files for the changes I have made
