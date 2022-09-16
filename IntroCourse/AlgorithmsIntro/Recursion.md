Something recursive is something that is self defined, say a number in the fibonacci sequence. Such a number is defined upon how a previous number in the sequence is defined like:

F_n = F_n-1 + F_n-2

n = 0 -> F = 0
n = 1 -> F = 1

An algorithm for the [[Hanois Tower]] can also be written. Moreover, an algorithm for finding if a string is a [[palindrome]] can be made with this tool.


A recursion algorithm will terminate if:
- The algorithm has a base case
- Each recursive call means that there are less recursive calls to the base case.

Some algorithms designed with this tool inspired by problems from [[AlgorithmsPdf1.pdf]] are provided in [[Task1]].