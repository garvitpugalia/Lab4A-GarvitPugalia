
## CS31/CS32/CS33 [the class this problem is for]

### Your Problem Title

*Contributed by Your Name*.

Your problem description. Remember to wrap in-line code in `ticks`!

#### Example

Example inputs and outputs, if helpful. If you don't have this, remove this section.

#### Solution

If you solution would benefit from a textual description, put that here. If you only want to provide the code, then remove these sentences!

```cpp
bool checkAnagram(const char a[], const char b[]) {
int string1[26] = { 0 };
int string2[26] = { 0 };
int count = 0;

while (a[count] != '\0') {
string1[a[count] - 'a']++;
count++;
}

count = 0;

while (b[count] != '\0') {
string2[b[count] - 'a']++;
count++;
}

for (int i = 0; i < 26; i++) {
if (string1[i] != string2[i])
return false;
}

return true;
}
```

---
