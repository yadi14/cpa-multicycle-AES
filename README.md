# Exhaustive-Search-on-Plaintext-and-Key
### Find all the m's which satisfies s(p + k) + s(p' + k) = m, for all possible p, p', k, and p != p' under GF(2^8) and AES's S-box.

number inside .txt file are in hexadecimal.

# Quick Start
* Create two new directories
```
mkdir p1p2_VERBOSE
mkdir p1p2_SIMPLIFY
```
* Compile c++ program
```
g++ P1P2K_VERBOSE.cpp -o p1p2k_verbose.out
g++ P1P2K_SIMPLIFY.cpp -o p1p2k_simplify.out
```
Since each program output a total of 32640 text files in each folder `p1p2_VERBOSE`, `p1p2_SIMPLIFY`, it may take several minutes to finish execution.

* Verify all text files in `p1p2_SIMPLIFY` with MATLAB
Directly run `verifyP1P2K.m` in MATLAB.

# Output Structure
For example, with p = 0x00, p' = 0x01
> k = 00	s(p^k) = 63, s(p'^k) = 7c, s(p^k)^s(p'^k) = 1f

# Software Tools
- g++ or MinGW
- MATLAB in __2020b__ or later version. `verifyP1P2K.m` calls function [readlines()](https://www.mathworks.com/help/matlab/ref/readlines.html), which is introduced on __2020b__.

# Software Used
All C++ programs have tested under g++ 7.5.0. MATLAB program has been tested on both MATLAB __2020b__ and __2021a__.
