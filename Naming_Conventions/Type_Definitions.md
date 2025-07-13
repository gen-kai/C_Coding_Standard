When defining custom types:
- Custom type names should use a delimiter-separated style, where the `underscore (_)` serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Custom types should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand, such as `u` in `u_int`).
- If a word is an actual alpha word or an abbreviation, it should only contain lower-case letters.

Example:
```c
typedef unsigned int u_int;
```
