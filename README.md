# Some Dubious and Pragmatic Benchmarks

This repo contains code for evaluating languages to use for string heavy programs (bioinformatics).

The benchmarks are not trying to find the fastest way to solve the problem of count the number of fields in the file, they are just meant to demonstrate the following:

1. Scriptability - How easy is it to read from stdin and split lines?
2. IO - Is there something inherently slow about how the language deals with IO?
3. String Ops - Are the builtins for doing string manipulations efficient, or do they just look pretty?
4. Lightweight Classes - can we cheaply create a class to hold data?
5. Array and String allocations - Does the compiler / interpreter optimize allocations? 
6. (Not yet done) C binding - How easy is it to use a c library?
7. (Not yet done) C interop - Is there a large cost to interacting with C libraries?

## Results

Lang | Time
---|---
Python3 | 0m8.211s
Perl | 0m13.431s
D | 0m14.854s
Nim | 0m6.265s

## Language version for results

Python 3.6
Perl 5.26
Nim 0.19
Dlang (dmd) v2.085.1
