
## CS31/CS32/CS33 [the class this problem is for]

### Your Problem Title

*Contributed by Your Name*.

Your problem description. Remember to wrap in-line code in `ticks`!

#### Example

Example inputs and outputs, if helpful. If you don't have this, remove this section.

#### Solution

If you solution would benefit from a textual description, put that here. If you only want to provide the code, then remove these sentences!

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
