General rules when declaring/defining a function:
- Function names should use PascalCase naming style, where the first letter of each word is written in upper-case and there are no delimiters between words.
- All words in custom types must be concise and clear to understand.
- Constant values' names should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand).
- Function parameters' names should follow naming conventions for the said constructs (e.g., variables should be named as defined by variable naming conventions, etc.).
- Function parameters' names should clearly indicate their purpose.

Example:
```c
int SetIntVarValue(int varToSet, int valueToBeSet);
```
---

When declaring/defining functions that return boolean values:
- All general rules apply.
- The name of the function should start with the word `Is`.

Example:
```c
bool IsVarEqualToValue(int varToCompare, int valueToBeComparedWith);
```
---

When declaring/defining functions that operate on pointers:
- All general rules apply.
- The sole exception to the rule about Function parameters' names is pointers: they should use naming conventions for variables as they won't produce meaningful names if named as pointers in generalized cases (e.g., p_varName).

Example:
```c
int ModifyPointer(void *pointerToModify, int valueToModifyBy);
```
