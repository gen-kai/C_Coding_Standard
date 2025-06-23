# C Coding Standard
- [Overview](#overview)
- [Naming Conventions](#naming-conventions)

## Overview

This repository aims to standardize my C code practices as much as possible.</br>
Here, I will describe how I name different language constructs, the techniques I use, and the rules I follow.</br>

This document consists of several sections, each residing in a different directory.</br>
Each section consists of several subsections that are assembled into a single file, which represents the section.</br>
Those section files are then assembled into the resulting document (README.md).

## Naming Conventions
- [Section Overview](#section-overview)
- [Type Definitions](#type-definitions)
- [Preprocessor Directives and Macros](#preprocessor-directives-and-macros)
- [Function Names](#function-names)

### Section Overview

This section describes naming conventions I use when coding in C.

### Type Definitions

When defining custom types using syntax

```c
typedef type_name new_type_name
```
- Custom type names should use a delimiter-separated style, where the `underscore (_)` serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Custom types should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `u` in `u_int`).
- If a word is an actual alpha word or an abbreviation, it should only contain lower-case letters.

### Preprocessor Directives and Macros

### Function Names

Function names
