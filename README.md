# C Coding Standard
- [Overview](#overview)
- [Naming Conventions](#naming-conventions)
  - [Type Definitions](#type-definitions)
  - [Preprocessor Directives and Macros](#preprocessor-directives-and-macros)
  - [Constants](#constants)
  - [Variables](#variables)
  - [Pointers](#pointers)
  - [Structures](#structures)
  - [Functions](#functions)
- [Formatting](#formatting)
  - [ClangFormat](#clangformat)
- [Comments](#comments)
- [Program Files Layout/Structure](#program-files-layoutstructure)
- [Core Principles](#core-principles)

# Overview

This repository aims to standardize my C code practices as much as possible.</br>
Here, I will describe how I name different language constructs, the techniques I use, and the rules I follow.</br>

This document consists of several sections, each residing in a different directory.</br>
Each section consists of several subsections that are assembled into a single file, which represents the section.</br>
Those section files are then assembled into the resulting document (README.md).

# Naming Conventions

This section describes naming conventions I use when coding in C.

## Type Definitions

When defining custom types:
- Custom type names should use a delimiter-separated style, where the underscore (`_`) serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Custom types should always consist of at least 2 words, including a suffix of `t` for type.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `u` in `u_int`).
- If a word is an actual alpha word or an abbreviation, it should only contain lower-case letters.

Example:

```c
typedef unsigned int u_int_t;
```

## Preprocessor Directives and Macros

When using a `#define` directive to define a constant value:
- Constant values' names should use a delimiter-separated style, where the underscore (`_`) serves as the delimiter to separate words.
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
- Constant values' names should use a delimiter-separated style, where the underscore (`_`) serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Constant values' names should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `MAX` in `MAX_TEXT_SIZE`).
- If a word is an actual alpha word or an abbreviation, it should only contain upper-case letters.

Example:

```c
const int MAX_TEXT_SIZE = 4000;
```

## Variables

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

## Pointers

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

## Structures

## Functions

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

# Formatting

This section describes formatting rules I follow when coding in C.

## ClangFormat

I use ClangFormat tools to format my code files.
All the settings I use can be found in [ClangFormat config file](Formatting/Formatting/.clang-format.md)

# Comments

# Program Files Layout/Structure

# Core Principles

This section describes core principles I follow when coding in C.
