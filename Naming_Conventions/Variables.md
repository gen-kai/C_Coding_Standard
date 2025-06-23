General rules when declaring/defining a variable:
- Variable names should use camelCase naming style, where the first letter of each word, except for the first, is written in upper-case and there are no delimiters between words.
- All words in variable names must be concise and clear to understand.
- Variable names should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand).
- Variable names should clearly indicate their purpose.

Example:
```c
u_int currentPacketSize;
```
---

When declaring/defining boolean variables:
- All general rules apply.
- The name of the variable should start with the word `is`.

Example:
```c
bool isTextLenLargerThanMax = false;
```
