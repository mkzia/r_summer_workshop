# Choosing which statements to execute

```r
if (some condition is TRUE) {
    do something
} else if (if some other condition is TRUE) {
    do something
} else if (if some other condition is TRUE) {
    do something
}
else {
    do something
}
```

- put the condition inside `()`
- `{}` are used to separate the body
- can have many `else if` tests
- do not need `else`
- conditions can be nested

## Examples

| pH Level | Solution Category |
|----------|-------------------|
| 0-4      | Strong acid       |
| 5-6      | Weak acid         |
| 7        | Neutral           |
| 8-9      | Weak base         |
| 10-14    | Strong base       |

```r
ph = 4
if (ph < 7.0) {
    print(paste(ph, "is acidic.")) 
}
```

```r
ph = 4
if (ph < 7.0) {
    print(paste(ph, "is acidic.")) 
    print('You should be careful with that!')
}

```

```r
ph = 4
if (ph < 7.0) {
    print(paste(ph, "is acidic.")) 
} else if (ph > 7.0) {
    print(paste(ph, "is basic."))  
} else {
    print(paste(ph, "is neutral."))  
}
```

- What is wrong with the following code?

```r
ph = 2
if (ph < 7.0) {
    print(paste(ph, "is acidic.")) 
} else if (ph < 3.0) {
    print(paste(ph, "is VERY acidic.")) 
}
```
