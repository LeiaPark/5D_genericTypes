# 5D_genericTypes

exercises in using classes that are parameterized with
generic types

## in [`Pair` example](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/2019-04-05_PairOfGenerics)

For each item in this section, find exemplifying code in the `Pair` example.
>For easy reference in the future, take advantage of
GitHub's "Copy permalink" command: click on a line number,
then click on the resulting ellipsis. Use the permalink as the URL
in [GitHub-Flavored Markdown](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#links).


- (an example of this task) the declaration of a `main` method:
```
public static void main(String[] args)
```
in [UserSavedByCompiler](https://github.com/stuyvesant-cs/solutionsHolmes/blob/21b641c9dda3c43d3e71de138c24c29f11687d88/2019-04-05_PairOfGenerics/UserSavedByCompiler.java#L11)


- definition that a class / type that is parameterized by a generic type, `T`:
```
public class Pair<T> 
```
in [Pair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/Pair.java#L8)


- declaration of a variable that can hold a reference to an instance
of such a class:
```
private T first;
private T second;
```
in [Pair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/Pair.java#L10)


- assignment to such a variable:
```
this.first =  first;
this.second = second;
```
in [Pair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/Pair.java#L14)


- declaration of a method that returns an instance of such a type:
```
public T getFirst()  { return first; }
public T getSecond() { return second; }
```
in [Pair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/Pair.java#L22)


- successful instantiation of an instance of such a class:
```
Pair<Integer> newPair = new Pair<Integer>(givenPair.getFirst() + givenPair.getSecond(), givenPair.getFirst());
```
in [FibPair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/FibPair.java#L57)


- *un*successful instantiation of an instance of such a class,
caught by the compiler:
```
return new Pair<String>(givenPair.getFirst() + givenPair.getSecond(), givenPair.getFirst());
```
in [FibPair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/FibPair.java#L60)


- a variable that can hold a reference to an instance of the generic type
in a class / type that is parameterized by a generic type:
```
Pair<Integer> newPair = new Pair<Integer>(givenPair.getFirst() + givenPair.getSecond(), givenPair.getFirst());
```
in [FibPair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/FibPair.java#L57)


- the declaration of a method or constructor that accepts a parameter of a generic type:
```
private static Pair<Integer> nextPairAfter( Pair<Integer> givenPair)
```
in [FibPair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/FibPair.java#L56)


- the declaration of a method that returns a value of a generic type:
```
private static Pair<Integer> nextPairAfter( Pair<Integer> givenPair)
```
in [FibPair](https://github.com/LeiaPark/5D_genericTypes/blob/master/FibPair/FibPair.java#L56)


