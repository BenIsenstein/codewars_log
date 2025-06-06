# Sum of Intervals

[Train this kata](https://www.codewars.com/kata/52b7ed099cdc285c300001cd)

Completed on February 11, 2025 at 10:01:57 PM UTC

Write a function called `sumIntervals`/`sum_intervals` that accepts an array of intervals, and returns the sum of all the interval lengths. Overlapping intervals should only be counted once.

### Intervals

Intervals are represented by a pair of integers in the form of an array. The first value of the interval will always be less than the second value. Interval example: `[1, 5]` is an interval from `1` to `5`. The length of this interval is `4`.

### Overlapping Intervals

List containing overlapping intervals:

```c -- actual language id doesn't matter -- just want syntax highlighting
[
   [1, 4],
   [7, 10],
   [3, 5]
]
```

The sum of the lengths of these intervals is `7`. Since `[1, 4]` and `[3, 5]` overlap, we can treat the interval as `[1, 5]`, which has a length of `4`.

### Examples:

```c -- idem
sumIntervals( [
   [1, 2],
   [6, 10],
   [11, 15]
] ) => 9

sumIntervals( [
   [1, 4],
   [7, 10],
   [3, 5]
] ) => 7

sumIntervals( [
   [1, 5],
   [10, 20],
   [1, 6],
   [16, 19],
   [5, 11]
] ) => 19

sumIntervals( [
   [0, 20],
   [-100000000, 10],
   [30, 40]
] ) => 100000030
```

### Tests with large intervals

Your algorithm should be able to handle large intervals. All tested intervals are subsets of the range `[-1000000000, 1000000000]`.

~~~if:lambdacalc
### Encodings

purity: `LetRec`  
numEncoding: `ScottBinary` ( subsets are actually in range `[0, 2000]` )  
export constructor `Pair` for your `Pair` encoding  
export constructors `nil, cons` for your `List` encoding  
~~~
