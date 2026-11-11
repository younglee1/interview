---

**Request Flag Check**

Each inbound request to a search ingestion service is tokenized into a string array `tokens`. The security team maintains a list of blocked tokens as a string array `blocked`.

A request must be flagged when **two or more entries** in `tokens` are identical to some token in `blocked`. Implement `needsFlag(tokens, blocked)`. It returns `true` if the request must be flagged and `false` otherwise.

Matching rules:

- An entry counts only if the whole string is equal to a token in `blocked`. Partial matches, prefixes, and substrings do not count.
- Every position in `tokens` is counted separately. If the same token appears twice in `tokens`, it counts twice.
- Repeated tokens in `blocked` have no extra effect.
- The matching entries do not need to be adjacent, and their order does not matter.

**Example 1**

```
Input:  tokens = ["hello","world","leetcode"], blocked = ["world","hello"]
Output: true
```

`"hello"` and `"world"` are both on the blocked list. That makes two matching entries.

**Example 2**

```
Input:  tokens = ["hello","programming","fun"], blocked = ["world","programming","leetcode"]
Output: false
```

Only `"programming"` matches, so there is just one matching entry.

**Example 3**

```
Input:  tokens = ["spam","spam"], blocked = ["spam"]
Output: true
```

The same token fills two positions, so it counts as two matching entries.

**Example 4**

```
Input:  tokens = ["flag","flagging"], blocked = ["flag"]
Output: false
```

`"flagging"` is not equal to `"flag"`, so only one entry matches.

**Constraints**

- `1 <= tokens.length, blocked.length <= 10^5`
- `1 <= tokens[i].length, blocked[i].length <= 15`
- All strings consist only of lowercase English letters.



**Solution**

```
class Solution {
    public boolean needsFlag(String[] tokens, String[] blocked) {
        
    }
}
```
