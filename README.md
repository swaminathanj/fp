# Functional Programming Principles

Functional Programming with Haskell and mainstream languages

**Online compiler**: https://onecompiler.com/haskell

**Hackerrank problems**: https://www.hackerrank.com/domains/fp

**Reference texts**

1. Richard Bird, “[Thinking Functionally with Haskell](https://elhacker.info/manuales/Lenguajes%20de%20Programacion/Haskell/Thinking%20Functionally%20With%20Haskell.pdf)”, Cambridge University Press, 2014.
   - **Chapterwise programs from** https://www.cs.ox.ac.uk/publications/books/functional/
2. Rebecca Skinner, “Effective Haskell - Solving Real-World Problems with Strongly Typed Functional Programming”, Pragmatic Bookshelf, 2023.
3. Richard S. Bird and Jeremy Gibbons, “Algorithm Design with Haskell”, Cambridge University Press, 2020.
4. David Mertz, “Functional Programming in Python”, O’Reilly, 2015.
5. John De Nero, “Composing Programs”. Online https://composingprograms.com/
6. Wampler Dean, “Functional Programming for Java Developers”, O’Reilly, 2011.

Functional Programming (FP) is a style or way of writing programs treating values and functions in some different way.

There are 4 core important things that you absolutely need to know.

1. Keep the functions and data totally separate. No side effect.

This is not an acceptable code in FP
```
let score = 456;
function addBonus() {
    score = score + 25;
    return score
}
```
whereas the following is preferred.
```
function addBonus(score) {
   return score + 25;
}
```

The second one is not referring to any global variable and the behavior can be reasoned easily.

2. Do not change the state much often. If you can avoid it, do it. Immutability.
```
greet = "hi"
greet = "hello"
greet = "hey there"
```
```
greet = "hi"
greetWed = "hello"
greetSat = "hey there"
```
3. Functions are treated as first class. First class citizens.
```
const addScore = function() {....}
```
4. 

5. 
