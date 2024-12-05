# Advent of Code 2024

In [Tokay](https://tokay.dev) v0.6.6.

## Logbook

- Day 1: Easy, some bugs
- Day 2: Medium, some bugs
- Day 3: Easy
- Day 4: Medium, many bugs
- Day 5: Easy, many bugs

## Found missing features for Tokay

- `list`
  - `copy`-function
  - `in` test, or `index`-function?
- `dict`
  - `copy`-function
  - `in` test, or `index`-function?
- `is void`-check, currently only `type(value) == "void"` is possible
- `for i, v in ((1, 2), (3, 4)) print(i, v)` (fails to compile)
- `enum`-iterator is not user-friendly
  - works: `for i in iter((1,2,3)).enum() print(i)`
  - fails: `for i in (1,2,3).enum() print(i)`
  - fails: `for i in enum((1,2,3)) print(i)`
