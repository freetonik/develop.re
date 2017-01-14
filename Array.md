An **array** is a [[data structure]], a collection of elements each identified by an index. An array is stored in such a way that the position of each element in memory can be computed from its index by a mathematical formula.

[[/uploads/cspr_0601.png]]
<small>An illustration of array access in Ruby from Computer Science Programming Basics in Ruby by by David Grossman, Gideon Frieder, Ophir Frieder</small>

### Alternative definitions
I. A data structure consisting of a group of elements that are accessed by indexing. In most programming languages each element has the same data type and the array occupies a contiguous area of storage. Most programming languages have a built-in array data type.<sup>1</sup>

### Examples

#### Array in JavaScript

```javascript
var years = [1950, 1960, 1970, 1980, 1990, 2000, 2010];
console.log(years[1]);
```

#### Array in C

```c
int main()
{
   int i;
   int arr[5] = {10,20,30,40,50};
 
   for (i=0;i<5;i++)
   {
      printf("value of arr[%d] is %d \n", i, arr[i]);
   }
 
}
```

#### Array in Swift

```swift
var someInts = [Int]()
print("someInts is of type [Int] with \(someInts.count) items.")
```

### Videos
1. [Khan Academy — Intro to Arrays (in JavaScript)](https://www.youtube.com/watch?v=gUOwZkL09BE)
2. [Learning programming: Arrays (in C)](https://www.youtube.com/watch?v=u3FZmUVT6V4) 

---
<div class="footnotes">
1. https://apcswshs.wikispaces.com/Arrays
2. 
</div>