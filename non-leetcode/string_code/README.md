# String Code

We are given a string text of length N consisting of the letters 'a', 'b' or 'c'. We can insert any of those letters before or after any letter in the string.

The goal is to insert letters into text so that it will follow the pattern "abcabca..." i.e. it should start with a letter 'a'. Letter 'a' should be followed by 'b', letter 'b' should be followed by 'c', and letter 'c' by 'a'. The string may end with any of those three letters. What is the minimum number of letters we need to insert into text?

**Write a function:**

```python
int solution(String text);
```

that, given a string text of length N, returns the minimum number of insertions needed to make text follow the described pattern.

**Examples:**

For text = "aabcc" we need to insert letters 'b' and c' between the pair of letters "a, and then insert letters 'a' and 'b' between the two letters C'. This way we obtain the string "abcabcabc" and the function should return 4.

For text = "abcabcabca", we do not need to insert any letters.

The string already follows the required pattern, so the function should return O. Note that text does not need to end with letter c.

For text = "bcaaa", letter 'a' should be inserted at the beginning of text, and then letters 'b' and 'c' should be inserted between the two pairs of letters a. This way we obtain the string "abcabcabca" and the function should return 5.

**Assume that:**

• N is an integer within the range `(1..100]`

• string text consists only of the following characters: `"a", "b" and/or c"`
