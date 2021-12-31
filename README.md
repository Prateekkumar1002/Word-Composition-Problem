# Word-Composition-Problem

ReadMe File

Word Composition Problem

•	Reads provided files (Input_01.txt and Input_02.txt) containing alphabetically sorted words list.

•	Identifies & display below given data in logs/console/output file

o	Longest compounded word

o	Second longest compounded word

o	Time taken to process the input file

Input 01 file contains small word list consisting following words.

Input 02 file contains long word list, consisting 100,000+ items

Approach:

There are so many ways to store the information and search the strings in given text file. We can implement with two logic dynamic programming (Intuition and Algorithm) and Trie with dynamic programming. I basically used trie data structure to implement the logic and find the longest and second longest word which is an ordered tree data structure and strings that share the common node for prefix and suffix. 
Firstly, I read the text file with mode “r” and create the list and declare it. Then strip, spilt and append and close the file
Define the node and initialize it and create the trie data structure and count it. And add each word to a trie data structure & add word length and sort the word length of word and get two longest words at first. And try to find the each word and check the prefix and that exists in the trie if exists then try to search for suffix and see the prefix and call recursively. If prefix and suffix both exists in the trie then that word is concatenated word and counts the incremented concatenated word at each time. If word is sorted with length of character then return the first two concatenated words.
