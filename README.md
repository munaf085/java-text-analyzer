# Build a text analyzer

A program that reads a sentence and reports on it: its characters, words and vowels, its longest word, the sentence in Title Case and reversed, and whether it is a **palindrome** (it reads the same backwards, ignoring spaces and case).

## Features

- Read a full sentence with `nextLine()`; ask again if it is empty.
- Print the number of characters and words.
- Count the vowels (a, e, i, o, u), in upper or lower case.
- Print the longest word and the sentence in Title Case.
- Print the sentence reversed, and whether it is a palindrome.
- Ask `Analyze another? (y/n)` and repeat on `y`.

## How to run

```
javac TextAnalyzer.java
java TextAnalyzer
```

## Sample run

```
=== Text Analyzer ===
Enter a sentence: Java is fun to learn
Characters: 20
Words: 5
Vowels: 7
Longest word: learn
Title case: Java Is Fun To Learn
Reversed: nrael ot nuf si avaJ
Palindrome: no
Analyze another? (y/n): y
Enter a sentence: Never odd or even
Characters: 17
Words: 4
Vowels: 6
Longest word: Never
Title case: Never Odd Or Even
Reversed: neve ro ddo reveN
Palindrome: yes
Analyze another? (y/n): n
Bye!
```

## What I used

- [`nextLine()`](/learn/java/basics/input-and-output/next-vs-nextline) and `trim()` to read a whole sentence
- [`split("\\s+")`](/learn/java/basics/strings/splitting-joining-and-parsing) to get the words
- [A loop over a String](/learn/java/basics/strings/looping-through-a-string) with `charAt` and `Character.isLetter`
- [`indexOf`](/learn/java/basics/strings/essential-string-methods) to test for a vowel
- [`substring`](/learn/java/basics/strings/substring), `toUpperCase` and `toLowerCase` for Title Case
- [`StringBuilder`](/learn/java/basics/strings/stringbuilder) with `append` and `reverse`
- A `while` loop with `continue` to skip empty lines
- The [ternary operator](/learn/java/basics/operators/ternary-operator) to print `yes` or `no`

## Author

Your name
