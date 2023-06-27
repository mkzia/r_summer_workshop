# Boolean Operators

- So far we have only written small programs that are a sequence of instructions. Sometimes you have to alter the sequential flow of a program to suit the needs of a particular situation.

## Boolean Type

- R has a built-in logical type that only has two values: `TRUE` and `FALSE`.

## Boolean Operators

- There are three basic Boolean operators: `&`, `|`, and `!`.

| Operator | What it does?                                        | Example                                                                   |
|----------|------------------------------------------------------|---------------------------------------------------------------------------|
| `&`    | TRUE if both a AND b are TRUE (logical conjunction)  | if is_teacher and is_active:   print('You can access')                    |
| `|`     | TRUE if either a OR b are TRUE (logical disjunction) | if is_superuser or (is_teacher and is active):    print('You can access') |
| `!`    | TRUE if the opposite of a is TRUE (logical negation) | if not is_superuser:   print('You cannot access')

```r
!TRUE
```

```r
!FALSE
```

```r
TRUE & TRUE
```

```r
FALSE & FALSE
```

```r
TRUE & FALSE
```

```r
FALSE & TRUE
```

```r
TRUE | TRUE
```

```r
FALSE | FALSE
```

```r
TRUE | FALSE
```

```r
FALSE | TRUE
```

```r
cold = TRUE
windy = FALSE

(!cold) & windy # It is not cold and windy
!(cold &  windy) # 
```
