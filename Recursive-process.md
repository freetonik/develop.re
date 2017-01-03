A **recursive process** is a process of computation, characterized by a chain of _deferred_ operations. Carrying out this process requires that the interpreter keeps track of the operations to be performed later on. <sup>1</sup>

### Example
**Scheme:**
```scheme
(define (factorial n)
  (if (= n 1)
      1
      (* n (factorial (- n 1)))))
```

**JavaScript:**
```javascript
const factorial = (n) => {
  if (n === 0) {
    return 1;
  }
  return n * factorial(n-1);
}
```

[[/uploads/recursion.gif]]

---

1. Structure and Interpretation of Computer Programs, chapter 1.2