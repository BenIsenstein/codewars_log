# Strip Comments

[Train this kata](https://www.codewars.com/kata/51c8e37cee245da6b40000bd)

Completed on October 4, 2022 at 5:28:38 AM UTC

Complete the solution so that it strips all text that follows any of a set of comment markers passed in. Any whitespace at the end of the line should also be stripped out. 

**Example:**

Given an input string of:
```
apples, pears # and bananas
grapes
bananas !apples
```

The output expected would be:
```
apples, pears
grapes
bananas
```

The code would be called like so:

```javascript
var result = solution("apples, pears # and bananas\ngrapes\nbananas !apples", ["#", "!"])
// result should == "apples, pears\ngrapes\nbananas"

```

```kotlin
var result = solution("apples, pears # and bananas\ngrapes\nbananas !apples", charArrayOf('#', '!'))
// result should == "apples, pears\ngrapes\nbananas"

```

```coffeescript
result = stripComments("apples, pears # and bananas\ngrapes\nbananas !apples", ["#", "!"])
# result should == "apples, pears\nograpes\nbananas"

```

```ruby
result = solution("apples, pears # and bananas\ngrapes\nbananas !apples", ["#", "!"])
# result should == "apples, pears\ngrapes\nbananas"

```

```crystal
result = solution("apples, pears # and bananas\ngrapes\nbananas !apples", ["#", "!"])
# result should == "apples, pears\ngrapes\nbananas"

```

```python
result = strip_comments("apples, pears # and bananas\ngrapes\nbananas !apples", ["#", "!"])
# result should == "apples, pears\ngrapes\nbananas"

```

```csharp
string stripped = StripCommentsSolution.StripComments("apples, pears # and bananas\ngrapes\nbananas !apples", new [] { "#", "!" })
// result should == "apples, pears\ngrapes\nbananas"
```

```julia
result = stripcomments("apples, pears # and bananas\ngrapes\nbananas !apples", ["#", "!"])
# result should == "apples, pears\ngrapes\nbananas"
```

```factor
"apples, pears # and bananas\ngrapes\nbananas !apples"
"#!"
strip-comments ! "apples, pears\ngrapes\nbananas"
```

```scala
val res = stripComments("apples, pears # and bananas\ngrapes\nbananas !apples", Set('#', '!'))
// res should be "apples, pears\ngrapes\nbananas"
```

```php
$result = stripComments("apples, pears # and bananas\ngrapes\nbananas !apples", ['#', '!']);
// $result should be "apples, pears\ngrapes\nbananas"
```
