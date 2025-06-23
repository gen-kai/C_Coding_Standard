When using a `const` modifier to define a constant value:
- The constant value's names should use a delimiter-separated style, where the underscore (_) serves as the delimiter to separate words.
- All words in custom types must be concise and clear to understand.
- Custom types should always consist of at least 2 words.
- A word can be an actual alpha word, a number, or an abbreviation (only if this abbreviation is widely used and is clear to understand).
- If a word is an actual alpha word or an abbreviation, it should only contain upper-case letters.

Example:
```c
const uint16_t MAX_TEXT_SIZE 4000
```
