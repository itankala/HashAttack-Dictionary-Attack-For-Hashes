# HashAttack: A Dictionary Attack Tool for Hashes

## Description & Usage
A high speed dictionary attack implementation (700,000+ lines per second), that takes the following as input:

- A custom range of integers to generate within
- Method (either Leading Zeros or Straightforward)
- Output location for the generated .txt file

...and then generates a file with all the integers within a user-specified range, either by the Leading Zeros method (constant length of digits from start to end, such as 0001, 0002... → 9999) or the Straightforward method (varying digit length, such as 1, 2… → 9999); ideal in aiding dictionary attacks performed against a number-based pin system, or if the candidates to be tried are within—say—a specific range of contact numbers (example: if a specific network vendor's numbers start with either the digit 7 or 8, a list consisting of all integers 7000000000 → 8999999999 would be both more efficient and ideal in finding the correct possible candidate, than a list of the 0000000000 → 9999999999 range).

<div align="center">
<img src="https://github.com/SHUR1K-N/NumNinja-Number-Dictionary-Generator/blob/master/Images/CUI%20Example.png" >
<p>NumNinja.py CUI</p>
</div>

This project was created in Python, for experimental/observational purposes; and can also be aided with my own super fast numbered dictionary generator [**NumNinja**](https://github.com/SHUR1K-N/NumNinja-Number-Dictionary-Generator)  (2M+ lines per second) for numeric attacks.

## Optimization
The extremely high integer-generating speed is owed to the implementation of multiprocessing in this program (the regular version of the program works flawlessly, but the much faster multiprocessing version is still an active work in progress).

## Dependencies to PIP-Install
- **colorama** (for colors)
- **termcolor** (for colors)

------------

My website: http://bit.do/SHUR1KN