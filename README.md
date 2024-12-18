# Advent of Code 2024

In [Tokay](https://tokay.dev) v0.6.6.

## Logbook

- Day 1: Easy, some bugs
- Day 2: Medium, some bugs
- Day 3: Easy, this was a Tokay parsing delight :-D
- Day 4: Medium, many bugs
- Day 5: Easy, many bugs
- Day 6: Heavy, many bugs
- Day 7: Medium, one bug
- Day 8: Heavy, had problems to find
- Day 9: Part 1 was easy, part 2 took a day more for this to resolve...
- Day 10: Medium
- Day 11: Medium, had to rewrite all for part 2 and needed some research

## Found missing features for Tokay

- `list`
  - `copy`-function
  - `in` test, or `index`-function?
- `dict`
  - `copy`-function
  - `in` test, or `index`-function?
  - May not fallback to offset indexing!!!
- `is void`-check, currently only `type(value) == "void"` is possible
- `for i, v in ((1, 2), (3, 4)) print(i, v)` (fails to compile)
- `enum`-iterator is not user-friendly
  - works: `for i in iter((1,2,3)).enum() print(i)`
  - fails: `for i in (1,2,3).enum() print(i)`
  - fails: `for i in enum((1,2,3)) print(i)`
- Index out of bounds returns void, index on void should always return voi
  - `map[10][10]` on a map sized 5x5 should return void
- `list_pop() can't pop off empty list` should return just void!
