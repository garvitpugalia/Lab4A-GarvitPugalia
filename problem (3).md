
## CS32

### Recursively replace a certain character in a string

*Contributed by Garvit Pugalia*.

Write a recursive function `void replace(char* word, char from, char to)` to recursively traverse through the string `word` and replace all occurrences of the character `from` to the character `to`. 

#### Example

Input: "There is a small brick house down the road", 'a', 'b'
Output: "There is b smbll brick house down the robd"

#### Solution

```cpp
void replace(char* word, char from, char to) {
if (*word == '\0')
return;
if (*word == from)
*word = to;
replace(word + 1, from, to);
}
```

---
