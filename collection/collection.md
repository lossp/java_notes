## Collection

### Set

#### HashSet

HashSet implements the interface `Set`

There are some features about HashSet

- It only can be one null in the HashSet, or zero at all.

- There is no order in HashSet

- Duplicated values are not allowed

- Cannot use for loop, but Iterator and foreach can be used instead



About being exclusive. The `put` Method in HashSet is actually the method `putVal` of HashMap. HashMap is the fundamental data structure of HashSet. The way of keeping the value in HashSet exclusive is that `onlyIfAbsent` is true in the `putVal` method, which means if there is a same value coming into the HashSet, it will only replace the old one.

About HashSet order. The reason why the HashSet has no order is that in the method `putVal` in HashMap, the index is calculated by the size of the HashMap and hash. Therefore the index is almost a random number to us.

HashSet does not provide a `get()` method that takes a index as an arugment. Therefore, for loop is not working. On the other hand, Iterator is provided, which means we can go through the all set by Iterator or foreach.



#### TreeSet

TreeSet implements the interface `NavigableSet`,  which is the subclass of `Set`.

The basic data structure of `TreeSet` implments the interface `NavigableMap`, which is a subclass of `Map`. But the constructor of `TreeSet` used `TreeMap` by default.

First of all, TreeSet is a order collection. Because all the elements inserted into it must implement the `Comparable`. Therefore, all the data formed into a tree, which means ordering.

Of course, duplicate elements are not allowed in TreeSet. Because the default data structure in TreeSet is TreeMap, whose `put` method will update the element if there is an old one existed. Therefore, duplicate elements are not allowed.

There are some features about TreeSet

- the elements are placed in order
- the search cost is O(lgN)
- data structure rely on Red And Black Tree, It can be understood as a `dynamic search tree`
- element cannot be null, because the element must be `Comparable`, otherwise it will throw a NullPointerException
- TreeSet use `compareTo` method to see if two elements are the same.





### Map

#### HashMap

#### TreeMap



