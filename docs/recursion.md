# Recursion

---

## Construction of recursive solutions:

- How can you define the problem in terms of a smaller problem of the same type?
- How does each recursive call diminish the size of the problem?
- What instance(s) of the problem can serve as the base case(s)?
- As the problem size diminishes, will you reach this base case?

## Factorial of n

Problem: Compute the factorial of an integer n

#### Iterative definition:

```
factorial(n) = n * (n - 1) * (n - 2) * ... * 1
    for any integer n > 0

factorial(0) = 1
```
#### Iterative solution:
```
public int factorial(int x){
    int result = 1;
    for (int i = 2; i <= x; i++>) result *= i;
    return result;
}
```
#### Recurrence relation:

```
factorial(n) = n * factorial(n - 1)

```
#### Recursive solution

```
public int factorial(int x){
    if (x == 0) return 1; // base case
    return x * factorial(x -1);
}
```

## Writing a string backwards

Problem: Write a string of characters in reverse order

#### Iterative definition

```
writeBackwards(s) = s.lastChar + s.secondLastChar + ... + s.firstChar + ""

writeBackwards("") = "\0" // null terminator

```

#### Iterative solution

```
public String writeBackwards(String text){
    int length = text.length();
    StringBuffer reverseString = new StringBuffer();
    for (int i = length - 1; i >= 0; i --) reverseString.append(text.charAt(i));
    return reverseString;
}
```

#### Recurrence relation

```
writeBackwards(s) = s.lastChar + writeBackwards(s.removeLastChar);
```

#### Recursive solution






