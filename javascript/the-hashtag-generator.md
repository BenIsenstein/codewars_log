# The Hashtag Generator

[Train this kata](https://www.codewars.com/kata/52449b062fb80683ec000024)

Completed on September 2, 2021 at 4:31:27 AM UTC

The marketing team is spending way too much time typing in hashtags.   
Let's help them with our own Hashtag Generator!

Here's the deal:

- It must start with a hashtag (`#`).
- All words must have their first letter capitalized.

~~~if-not:cpp,rust
- If the final result is longer than 140 chars it must return `false`.
- If the input or the result is an empty string it must return `false`.
~~~

~~~if:cpp
- If the final result is longer than 140 chars it must return `std::nullopt`.
- If the input or the result is an empty string it must return `std::nullopt`.
~~~

~~~if:rust
- If the final result is longer than 140 chars it must return `None`.
- If the input or the result is an empty string it must return `None`.
~~~

## Examples

~~~if-not:cpp,rust
```
" Hello there thanks for trying my Kata"  =>  "#HelloThereThanksForTryingMyKata"
"    Hello     World   "                  =>  "#HelloWorld"
""                                        =>  false
```
~~~

~~~if:cpp
```
" Hello there thanks for trying my Kata"  =>  "#HelloThereThanksForTryingMyKata"
"    Hello     World   "                  =>  "#HelloWorld"
""                                        =>  std::nullopt
```
~~~

~~~if:rust
```
" Hello there thanks for trying my Kata"  =>  Some("#HelloThereThanksForTryingMyKata")
"    Hello     World   "                  =>  Some("#HelloWorld")
""                                        =>  None
```
~~~