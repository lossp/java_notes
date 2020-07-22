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





### Map

#### HashMap



