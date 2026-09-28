# LeetCode 319 - Bulb Switcher

## Problem Statement

There are `n` bulbs initially turned off.

You make `n` rounds. In the first round, you switch every bulb. In the second round, you switch every second bulb. In the third round, every third bulb, and so on.

After all rounds, return the number of bulbs that remain on.

## Example 1

### Input

```text
n = 3
```

### Output

```text
1
```

## Example 2

### Input

```text
n = 0
```

### Output

```text
0
```

## Example 3

### Input

```text
n = 1
```

### Output

```text
1
```

## Approach

A bulb is switched every time its position is a divisor of the round number.

Most numbers have divisors in pairs. For example, `12` has pairs `(1,12)`, `(2,6)`, and `(3,4)`.

Only **perfect squares** have an odd number of divisors because one divisor is repeated, such as `3 × 3 = 9`.

Therefore, only bulbs at perfect square positions remain on.

The number of perfect squares from `1` to `n` is `floor(sqrt(n))`.

## Algorithm

1. Find the integer square root of `n`.
2. Return the result.
3. The integer square root gives the number of perfect squares less than or equal to `n`.

## Time Complexity

`O(1)`

## Space Complexity

`O(1)`

## Key Concepts

* Math
* Perfect Squares
* Divisors
* Integer Square Root
* Number Theory

## Language

Python

## LeetCode Details

* **Problem:** 319
* **Title:** Bulb Switcher
* **Difficulty:** Medium

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
