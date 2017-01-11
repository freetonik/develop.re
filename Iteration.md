**Iteration** is a defined repetitive execution of code with changing state. In programming, a common form of iteration is a loop.

See also: [[Iterative process]].

### Iteration vs. Recursion

In contrasting iteration and [[recursion]], we must be careful not to confuse the notion of a [[recursive process]] with the notion of a _recursive procedure_. When we describe a procedure as recursive, we are referring to the syntactic fact that the procedure definition refers (either directly or indirectly) to the procedure itself. But when we describe a process as following a pattern that is, say, linearly recursive, we are speaking about how the process evolves, not about the syntax of how a procedure is written. It may seem disturbing that we refer to a recursive procedure such as `fact-iter` (see below) as generating an iterative process. However, the process really is iterative: Its state is captured completely by its three state variables, and an interpreter need keep track of only three variables in order to execute the process.<sup>1</sup>

```scheme
(define (factorial n)
  (fact-iter 1 1 n))

(define (fact-iter product counter max-count)
  (if (> counter max-count)
      product
      (fact-iter ( counter product)
                 (+ counter 1)
                 max-count)))
```

### Examples

#### A for-of loop in JavaScript

```javascript
for (var value of myArray) {
  console.log(value);
}
```

#### A do-while loop in C

```c
do {
  printf("value of a: %d\n", a);
  a = a + 1;
} while( a < 20 );
```

### Articles

1. [Structure and Implementation of Computer Programs, chapter 1.2.1: Linear Recursion and Iteration](https://mitpress.mit.edu/sicp/chapter1/node12.html)

---

<div class="footnotes">
1. Structure and Implementation of Computer Programs, chapter 1.2.1: Linear Recursion and Iteration
</div>