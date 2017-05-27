
## CS31

### Check if two C strings are anagrams

*Contributed by Garvit Pugalia*.

Write a function `bool checkAnagram(const char a[], const char b[])` to check if two strings are anagrams. You can assume that the string contains only alphabets a-z. An anagram is a word formed by rearranging the letters of another word. For example, "listen" is an anagram of "silent".

#### Example

checkAnagram("silent", "listen") == true

checkAnagram("computer", "compute") == false

checkAnagram("maths", "thames") == false

#### Solution

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
