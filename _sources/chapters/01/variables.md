# Variables

Variables give names to values (number, string, None). They are an identifier that labels a value for future reference. The value of a variable can be changed through assignment.

Variables must be assigned values before they can be used in expressions.

Variables names **MUST** follow certain rules:

1. A variable name must start with a letter and can be a combination of letters, digits, period(.)
and underscore(_). If it starts with period(.), it cannot be followed by a digit.
2. A variable name cannot start with a number or underscore (_)
3. Variable names are case-sensitive (`ph` and `pH` are two different names.)
4. Reserved words cannot be used as variables (TRUE, FALSE, NULL, if...)

## Variable Assignment

Variables are created by executing assignment statements.

```R
degrees_celsius = 26.0
degrees_celsius <- 26.0
```

This is called an assignment statement; we say that `degrees_celsius` is assigned the value `26.0`. Whenever Python sees a variable in an expression, it substitutes the value to which the variables refers:

```R
degrees_celsius = 26.0
9 / 5 * degrees_celsius + 32
```

Variables are called variables because their value can vary as the program executes.

```R
degrees_celsius = 15.5
9 / 5 * degrees_celsius + 32
```

## Gotchas

```r
a = 3.14
print(a)
```

```r
print = 3.14
print(print)
```
