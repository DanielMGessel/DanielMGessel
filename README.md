I was a computer programmer and in retirement I still enjoy it. Hopefully, my projects will gel
soon and be ready for sharing. I have a recreational interest in Symbolic Logic and enjoy
Puzzles that can be solved logically - from ‘pencil puzzles’ like
[sudoku](https://www.nikoli.co.jp/en/) and [Sorted Puzzles](https://sortedpuzzles.com/) books
to [Raf Peeters](https://smartgamesandpuzzles.com/) designs for Smart Games.

Below is an image from a
nearly ready for prototyping puzzle.
![An 8 by 4 square grid on the left, with labelled
connecttions and a set of 8 colored tiles, 2 by 2, on the right.](sq-01-09-2025.png)


And this is a bit of propositional proving based on
[“Mathematical Logic Through Python”](logicthrupython.org) using Unicode characters available
in the [JuliaMono](https://juliamono.netlify.app/) font.

```
--| ∨ commutivity
proof: x∨y ∴ y∨x
  ▶ ¬A∨A               [r1]
  A∨B ¬A∨C ▶ B∨C       [r2]
  x∨y                  [0]
  ¬x∨x ∵ r1            [1]
  y∨x ∵ r2 0 1

--| ∨ associativity
proof: x∨y∨z ∴ x∨(y∨z)
  A∨(B∨C) ▶ A∨B∨C         [r1]
  A∨B ▶ B∨A               [r2]
  x∨y∨z                   [0]
  z∨(x∨y) ∵ r2 0          [1]
  z∨x∨y ∵ r1 1            [2]
  y∨(z∨x) ∵ r2 2          [3]
  y∨z∨x ∵ r1 3            [4]
  x∨(y∨z) ∵ r2 4
```