General rules when declaring/defining a pointer:
- Pointer names should use camelCase naming style, where the first letter of each word, except for the first, is written in upper-case and there are no delimiters between words.
- Pointers should have a prefix of `p_` (meaning "pointer to"). The prefix is used to differentiate between pointers and actual variables. The number of `p_` prefixes indicates the level of indirection.
- All words in pointer names must be concise and clear to understand.
- Pointer names should always consist of at least 2 words, not including the prefix.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand).
- Pointer names should clearly indicate their purpose.
- If the pointer is created based on a variable, it should replicate the variable's name with the addition of the prefix(-es).

Example:
```c
int inputNumber = 9;
int* p_inputNumber = &inputNumber;
int** p_p_inputNumber = &p_inputNumber
```
