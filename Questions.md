# Lottery Winner - Longest Common Subsequence Optimization

## Problem Statement
HackerRankNews has distributed lottery tickets to everyone, and the winning lottery ID is printed in the newspaper as **winnerID**.

Each customer has a **lotteryID**, and to maximize their chances of winning, they can modify their **lotteryID** by performing up to **k** operations.

In **one operation**, a character in **lotteryID** can be changed to its **next or previous character** in the alphabet:
- The **next character** of `'a'` is `'b'`, `'b'` is `'c'`, and so on.
- The **previous character** of `'b'` is `'a'`, `'c'` is `'b'`, and so on.
- `'z'` wraps around to `'a'`, and `'a'` wraps around to `'z'`.

The goal is to **maximize** the length of the **longest common subsequence (LCS)** between **lotteryID** and **winnerID** after performing at most **k** operations.

## Function Description
Implement the function:

```python
def getMaximumLength(lottery: str, winnerID: str, k: int) -> int:
```

### Parameters:
- `lottery` (string): The customer's lottery ID.
- `winnerID` (string): The winning lottery ID.
- `k` (int): The maximum number of character modification operations allowed.

### Returns:
- **int**: The maximum possible length of the **longest common subsequence (LCS)** after at most **k** operations.

## Example

### Input:
```python
lottery = "fpelqanxyk"
winnerID = "hackerrank"
k = 6
```

### Optimal Modifications:
1. Change `'f'` → `'h'` → `"hpelqanxyk"`
2. Change `'p'` → `'h'` → `"hpelqanxyk"`
3. Change `'e'` → `'d'` → `"hpdiganxyk"`
4. Change `'l'` → `'c'` → `"hpciqanxyk"`
5. Change `'q'` → `'k'` → `"hpckpanxyk"`
6. Change `'a'` → `'o'` → `"hpokranxyk"`

### Final LCS:
The longest common subsequence between `"hpokranxyk"` and `"hackerrank"` is **7**.

### Output:
```python
7
```

## Constraints
- `1 ≤ len(lottery), len(winnerID) ≤ 1000`
- `0 ≤ k ≤ 1000`
- `lottery` and `winnerID` contain only lowercase English letters (`a-z`).

## Notes
- The operations can only be applied to `lottery`, not `winnerID`.
- The goal is to maximize the LCS after at most `k` operations.

## License
This project is open-source and free to use under the MIT License.

