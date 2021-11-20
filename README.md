# Exhaustive-Search-on-Plaintext-and-Key
## Find all the m's which satisfies s(p + k) + s(p' + k) = m, for all possible p, p', k, and p != p' under GF(2^8) and AES's S-box.

number inside .txt file are in hexadecimal.


# File Structure
For example, with p = 00, p' = 01
> k = 00	s(p^k) = 63, s(p'^k) = 7c, s(p^k)^s(p'^k) = 1f



# Software Tools
- g++ or MinGW
- MATLAB in __2020b__ or later version. *verifyP1P2K.m* calls function [readlines()](https://www.mathworks.com/help/matlab/ref/readlines.html), which is introduced on __2020b__.

# Software Used
### All C++ programs have tested under g++ 7.5.0. MATLAB program has been tested on both MATLAB __2020b__ and __2021a__.
