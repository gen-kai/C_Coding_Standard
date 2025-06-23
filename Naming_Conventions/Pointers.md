General rules when declaring/defining a pointer:
- Pointer names should use camelCase naming style, where the first letter of each word, except for the first, is written in upper-case and there are no delimiters between words + the prefix of `p_`. The prefix is used to differentiate between pointers and actual variables.
- All words in pointer names must be concise and clear to understand.
- Pointer names should always consist of at least 2 words, not including the prefix.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand).
- Pointer names should clearly indicate their purpose.
- If the pointer is created based on a variable, it should replicate the variable's name with the addition of the prefix.

Example:
```c
u_int inputNumber = 9;
u_int *p_inputNumber = &inputNumber;
```
