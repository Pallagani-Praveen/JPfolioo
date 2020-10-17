## Hai this is Solutions Page 

[Today Leetcode Question](https://leetcode.com/explore/challenge/card/october-leetcoding-challenge/561/week-3-october-15th-october-21st/3498/)

Solution For The Today's Question : -

```python
  class Solution(object):
    def findRepeatedDnaSequences(self, s):
        """
        :type s: str
        :rtype: List[str]
        """
        freaks = collections.Counter([ s[i:i+10] for i in range(len(s)-9)])
        return [ key for key in freaks if freaks[key]>1 ]
```
