## solutions of todays challenge

```python 
class Solution(object):
    def asteroidCollision(self, asts):
        """
        :type asteroids: List[int]
        :rtype: List[int]
        """
        stack = []
        for new in asts:
            while stack and new < 0 < stack[-1]:
                if abs(new)>stack[-1]:
                    stack.pop()
                elif abs(new)==stack[-1]:
                    stack.pop()
                    break
                else:
                    break
            else:
                stack.append(new)
        return stack
```

[Explanation Video Link](#) 
