# sudoku-js

Sudoku solver and generator

## Usage

```javascript
var _ = Sudoku.empty;
var q = [
    _,_,_,1,9,_,_,3,6,
    _,_,6,_,3,7,1,_,_,
    3,1,9,_,_,2,8,_,_,
    1,6,_,_,8,_,_,9,3,
    _,_,_,4,_,9,_,_,_,
    9,8,_,_,1,_,_,7,5,
    7,9,8,_,_,1,3,_,_,
    _,_,1,_,5,8,9,_,_,
    _,_,_,9,4,_,_,1,8
  ];

console.log(Sudoku.beautify(Sudoku.solve(q)));

// 8,7,2,1,9,4,5,3,6,
// 5,4,6,8,3,7,1,2,9,
// 3,1,9,5,6,2,8,4,7,
// 1,6,7,2,8,5,4,9,3,
// 2,5,3,4,7,9,6,8,1,
// 9,8,4,3,1,6,2,7,5,
// 7,9,8,6,2,1,3,5,4,
// 4,3,1,7,5,8,9,6,2,
// 6,2,5,9,4,3,7,1,8
```

## Performance

This solver is using the **elimination methods**, and the **backtracking**.

Almost all sudoku puzzles are solved in **50ms**, but some puzzles take *1000ms* or longer
