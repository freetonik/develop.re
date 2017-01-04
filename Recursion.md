**Recursion** is a way of defining solutions to problems in which the solution is applied inside its own definition. In other words, the solution depends on solutions to smaller instances of the same problem.

In programming, recursion usually means that a function calls itself until it doesn't.

_See also: [[Recursive process]]._

[[/uploads/0DaD5.jpg]]

### Alternative explanations
Recursion is the process of defining a problem (or the solution to a problem) in terms of (a simpler version of) itself.<sup>1</sup>

Recursion is a technique of designing algorithms to solve a problem by solving a smaller instance of the same problem, unless the problem is so small that we can just solve it directly.<sup>2</sup>

### Examples

#### Factorial in Java

```java
public int fib(int n) {
  if(n <= 1) {
    return n;
  } else {
    return fib(n - 1) + fib(n - 2);
  }
}
```

#### Sum of natural numbers in C

```c
int sum(int num)
{
  if (num!=0)
    return num + sum(num-1);
  else
    return num;
}
```

#### Palindrome check in JavaScript

```javascript
const isPalindrome = (str) => {
  const strLen = str.length;
  if (strLen === 0 || strLen === 1) {
    return true;
  }

  if (str[0] === str[strLen - 1]) {
    return isPalindrome( str.slice(1, strLen - 1) );
  }
  
  return false;
};
```

### Articles

1. [Hello recursion! / Learn You a Haskell for Great Good!](http://learnyouahaskell.com/recursion)
2. [Properties of recursive algorithms](https://www.khanacademy.org/computing/computer-science/algorithms/recursive-algorithms/a/properties-of-recursive-algorithms)

### Videos

1. [Recursion and recursive functions in JavaScript / Hexlet](https://www.youtube.com/watch?v=vLhHyGTkjCs)
2. [What on Earth is Recursion? / Computerphile](https://www.youtube.com/watch?v=Mv9NEXX1VHc)
3. [Recursion / Fun Fun Function](https://www.youtube.com/watch?v=k7-N8R0-KY4)
4. [Fibonacci Programming / Computerphile](https://www.youtube.com/watch?v=7t_pTlH9HwA)


---
<div class="footnotes">
1.[[https://www.cs.utah.edu/~germain/PPS/Topics/recursion.html]]
<br>
2.[[https://www.khanacademy.org/computing/computer-science/algorithms/recursive-algorithms/a/recursion]]
</div>