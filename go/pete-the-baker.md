# Pete, the baker

[Train this kata](https://www.codewars.com/kata/525c65e51bf619685c000059)

Completed on January 25, 2024 at 5:07:28 AM UTC

Pete likes to bake some cakes. He has some recipes and ingredients. Unfortunately he is not good in maths. Can you help him to find out, how many cakes he could bake considering his recipes?

~~~if-not:factor,cpp,rust
Write a function `cakes()`, which takes the recipe (object) and the available ingredients (also an object) and returns the maximum number of cakes Pete can bake (integer). For simplicity there are no units for the amounts (e.g. 1 lb of flour or 200 g of sugar are simply 1 or 200). Ingredients that are not present in the objects, can be considered as 0.
~~~
~~~if:factor
Write a word `cakes`, which takes a recipe (assoc) and the available ingredients (also an assoc) and returns the maximum number of cakes Pete can bake (integer). For simplicity there are no units for the amounts (e.g. 1 lb of flour or 200 g of sugar are simply 1 or 200). Ingredients for the recipe that are not present can be considered as 0.
~~~
~~~if:cpp
Write a function `cakes()`, which takes the recipe (unordered_map<string, int>) and the available ingredients (also an unordered_map<string, int>) and returns the maximum number of cakes Pete can bake (integer). For simplicity there are no units for the amounts (e.g. 1 lb of flour or 200 g of sugar are simply 1 or 200). Ingredients that are not present in the objects, can be considered as 0.
~~~
~~~if:rust
Write a function `cakes()`, which takes the recipe (HashMap<&str, u32>) and the available ingredients (also a HashMap<&str, u32>) and returns the maximum number of cakes Pete can bake (u32). For simplicity there are no units for the amounts (e.g. 1 lb of flour or 200 g of sugar are simply 1 or 200). Ingredients that are not present in the objects, can be considered as 0.
~~~

Examples:

```javascript
// must return 2
cakes({flour: 500, sugar: 200, eggs: 1}, {flour: 1200, sugar: 1200, eggs: 5, milk: 200}); 
// must return 0
cakes({apples: 3, flour: 300, sugar: 150, milk: 100, oil: 100}, {sugar: 500, flour: 2000, milk: 2000}); 
```
```coffeescript
# must return 2
cakes({flour: 500, sugar: 200, eggs: 1}, {flour: 1200, sugar: 1200, eggs: 5, milk: 200}) 
# must return 0
cakes({apples: 3, flour: 300, sugar: 150, milk: 100, oil: 100}, {sugar: 500, flour: 2000, milk: 2000}) 
```
```python
# must return 2
cakes({flour: 500, sugar: 200, eggs: 1}, {flour: 1200, sugar: 1200, eggs: 5, milk: 200})
# must return 0
cakes({apples: 3, flour: 300, sugar: 150, milk: 100, oil: 100}, {sugar: 500, flour: 2000, milk: 2000})
```
```haskell
cakes [("flour",500), ("sugar",200), ("eggs",1)] [("flour",1200), ("sugar",1200), ("eggs",5), ("milk",200)]  `shouldBe` 2
cakes [("apples",3), ("flour",300), ("sugar",150), ("milk",100), ("oil",100)] [("sugar",500), ("flour",2000), ("milk",2000)] `shouldBe` 0
```
```factor
{ { "flour" 500 } { "sugar" 200 } { "eggs" 1 } } { { "flour" 1200 } { "sugar" 1200 } { "eggs" 5 } { "milk" 200 } } cakes ->  2
{ { "apples" 3 } { "flour" 300 } { "sugar" 150 } { "milk" 100 } { "oil" 100 } } { { "sugar" 500 } { "flour" 2000 } { "milk" 2000 } } cakes -> 0
```
```cpp
// must return 2
cakes({{"flour", 500}, {"sugar", 200}, {"eggs", 1}}, {{"flour", 1200}, {"sugar", 1200}, {"eggs", 5}, {"milk", 200}});
// must return 0
cakes({{"apples", 3}, {"flour", 300}, {"sugar", 150}, {"milk", 100}, {"oil", 100}}, {{"sugar", 500}, {"flour", 2000}, {"milk", 2000}});
```
```rust
// must return 2
cakes(HashMap::from([("flour", 500), ("sugar", 200), ("eggs", 1)]), HashMap::from([("flour", 1200), ("sugar", 1200), ("eggs", 5), ("milk", 200)]))
// must return 0
cakes(HashMap::from([("apples", 3), ("flour", 300), ("sugar", 150), ("milk", 100), ("oil", 100)]), HashMap::from([("sugar", 500),("flour", 2000), ("milk", 2000)]))
```