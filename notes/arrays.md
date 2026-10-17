# Arrays

## Key idea

A contiguous block of memory. Fast access by index, slow insert/delete in the middle.

## Complexity

| Operation        | Time           |
| ---------------- | -------------- |
| Access by index  | O(1)           |
| Search           | O(n)           |
| Insert at end    | O(1) amortized |
| Insert in middle | O(n)           |

## Code

```python
arr = [1,2,3]
arr.append(4)   # O(1) amortized
arr.insert(0,0) # O(n), shifts everything
```

## Gotchas

- Off-by-one errors with indices
- Dynamic array resize by doubling, which is why append is _amortized_ O(1)

## Sources

- [Video: Arrays (CS50)](https://example.com)
