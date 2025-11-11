# Rectangle into Squares

[Train this kata](https://www.codewars.com/kata/55466989aeecab5aac00003e)

Completed on January 3, 2021 at 7:18:11 AM UTC

The drawing below gives an idea of how to cut a given "true" rectangle into squares ("true" rectangle meaning that the two dimensions are different).

<svg style="max-width: 500px" xmlns="http://www.w3.org/2000/svg" viewbox="0 0 600 400" xmlns:bx="https://boxy-svg.com">
  <defs/>
  <rect x="82.87" y="43.571" width="300" height="300" style="stroke: rgb(0, 0, 0); fill: rgb(169, 0, 0);"></rect>
  <rect x="382.87" y="43.571" width="200" height="200" style="stroke: rgb(0, 0, 0); fill: rgb(35, 108, 0);"></rect>
  <rect x="382.87" y="243.571" width="100" height="100" style="stroke: rgb(0, 0, 0); fill: rgb(0, 8, 124);"></rect>
  <rect x="482.87" y="243.571" width="100" height="100" style="fill: rgb(122, 0, 78); stroke: rgb(151, 148, 148); stroke-width: 0px;"></rect>
  <path style="stroke: rgb(151, 148, 148); stroke-width: 2px; fill: rgb(125, 125, 125);" d="M 182.87 43.571 L 182.87 343.571"></path>
  <path style="stroke: rgb(151, 148, 148); stroke-width: 2; fill: rgb(122, 122, 122);" d="M 282.87 43.571 L 282.87 343.571"></path>
  <path style="stroke: rgb(151, 148, 148); stroke-width: 2; fill: rgb(125, 125, 125);" d="M 382.87 43.571 L 382.87 343.571"></path>
  <path style="stroke: rgb(151, 148, 148); stroke-width: 2; fill: rgb(122, 122, 122);" d="M 482.87 43.571 L 482.87 343.566"></path>
  <path style="stroke: rgb(151, 148, 148); stroke-width: 2; fill: rgb(120, 120, 120);" d="M 582.87 143.571 L 82.87 143.571"></path>
  <path style="stroke: rgb(151, 148, 148); stroke-width: 2; fill: rgb(122, 122, 122);" d="M 582.87 243.571 L 82.87 243.571"></path>
  <text style="fill: rgb(255, 255, 255); font-family: Arial, sans-serif; font-size: 28px; white-space: pre;" x="422.254" y="301.793">1</text>
  <text style="fill: rgb(255, 255, 255); font-family: Arial, sans-serif; font-size: 28px; white-space: pre; stroke-width: 1;" x="525.528" y="303.929">1</text>
  <text style="fill: rgb(255, 255, 255); font-family: Arial, sans-serif; font-size: 28px; white-space: pre;" x="442.758" y="152.969">2² = 4</text>
  <text style="fill: rgb(255, 255, 255); font-family: Arial, sans-serif; font-size: 28px; white-space: pre;" x="196.71" y="201.836">3² = 9</text>
</svg>

Can you translate this drawing into an algorithm?

You will be given two dimensions 

1. a positive integer length
2. a positive integer width

You will return a collection or a string (depending on the language; Shell bash, PowerShell, Pascal and Fortran return a string) with the size of each of the  squares.

#### Examples in general form:

(depending on the language)
```
  sqInRect(5, 3) should return [3, 2, 1, 1]
  sqInRect(3, 5) should return [3, 2, 1, 1]
  
  You can see examples for your language in **"SAMPLE TESTS".**
```

#### Notes:

- `lng == wdth` as a starting case would be an entirely different problem and the drawing is planned to be interpreted with `lng != wdth`. (See kata, Square into Squares. Protect trees! http://www.codewars.com/kata/54eb33e5bc1a25440d000891 for this problem). 

  When the initial parameters are so that `lng` == `wdth`, the solution `[lng]` would be the most obvious but not in the spirit of this kata   so, in that case, return `None`/`nil`/`null`/`Nothing` **or**
  return `{}` with C++, `[]` with Perl, Raku.
 - In that case the returned structure of **C** will have its `sz` component equal to `0`. 
 - Return the string `"nil"` with Bash, PowerShell, Pascal and Fortran.



