General rules when declaring/defining a function:
- Function names should use PascalCase naming style, where the first letter of each word is written in upper-case and there are no delimiters between words.
- All words in function names must be concise and clear to understand.
- Function names should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand).
- Function parameters' names should follow naming conventions for the said constructs (e.g., variables should be named as defined by variable naming conventions, etc.).
- Function parameters' names should clearly indicate their purpose.

Example:
```c
bool SetIntVarValue(int* p_varToSet, int valueToBeSet);
```
---
When declaring/defining functions that are used as operands in `if ()` statements:
- All general rules apply.
- The name of the function should start with the word `Is`.

Example:
```c
bool IsVarEqualToValue(int varToCompare, int valueToBeComparedWith);
```
