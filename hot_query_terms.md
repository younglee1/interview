---

# Hot Query Terms

A search platform collects query terms from recent traffic into a string array `terms`. The analytics team wants the `k` hottest terms for a dashboard.

Implement `topKHotTerms(terms, k)`. It returns a list of `k` terms chosen by the ranking rules below.

Ranking rules:

- A term with a higher frequency ranks higher.
- If two terms have the same frequency, the lexicographically smaller term ranks higher.
- Frequency is the number of times a term appears in `terms`.
- The returned list must be ordered from highest rank to lowest rank.

**Example 1**

```
Input:  terms = ["i","love","leetcode","i","love","coding"], k = 2
Output: ["i","love"]
```

`"i"` and `"love"` both appear twice. The remaining terms appear once. Between the two tied terms, lexicographical order places `"i"` before `"love"`.

**Example 2**

```
Input:  terms = ["the","day","is","sunny","the","the","the","sunny","is","is"], k = 4
Output: ["the","is","sunny","day"]
```

Frequencies are `"the"`: 4, `"is"`: 3, `"sunny"`: 2, `"day"`: 1.

**Example 3**

```
Input:  terms = ["a","b","a","c","b","a"], k = 2
Output: ["a","b"]
```

`"a"` appears three times and `"b"` appears twice, so they are the top two terms.

**Constraints**

- `1 <= terms.length <= 500`
- `1 <= terms[i].length <= 10`
- `terms[i]` consists only of lowercase English letters
- `1 <= k <= number of unique terms`



**Solution**

```
class Solution {
    public List<String> topKHotTerms(String[] terms, int k) {
        
    }
}
```
