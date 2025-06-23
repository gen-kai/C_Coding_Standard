# Naming Conventions
- [Section Overview](#section-overview)
- [Type Definitions](#type-definitions)
- [Preprocessor Directives and Macros](#preprocessor-directives-and-macros)
- [Constants](#constants)
- [Functions](#functions)

## Section Overview

This section describes naming conventions I use when coding in C.

## Type Definitions

When defining custom types:
- Custom type names should use a delimiter-separated style, where the `underscore (_)` serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Custom types should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `u` in `u_int`).
- If a word is an actual alpha word or an abbreviation, it should only contain lower-case letters.

Example:

```c
typedef unsigned int u_int
```

## Preprocessor Directives and Macros

When using a `#define` directive to define a constant value:
- Constant values' names should use a delimiter-separated style, where the underscore (_) serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Constant values' names should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `MAX` in `MAX_TEXT_SIZE`).
- If a word is an actual alpha word or an abbreviation, it should only contain upper-case letters.

Example:

```c
#define MAX_TEXT_SIZE 4000
```

## Constants

When using a `const` modifier to define a constant value:
- Constant values' names should use a delimiter-separated style, where the underscore (_) serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Constant values' names should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `MAX` in `MAX_TEXT_SIZE`).
- If a word is an actual alpha word or an abbreviation, it should only contain upper-case letters.

Example:

```c
const int MAX_TEXT_SIZE = 4000;
```

## Functions

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
