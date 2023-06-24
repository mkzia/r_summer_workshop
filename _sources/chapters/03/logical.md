# Relational Operators

- A relational operator converts an expression into a boolean type, which is a basic Python data type.

- Assume `a=1` and `b=1`

| Relational Operators | What it does?                                | Example       |
|----|---------------------------------------------|---------------|
| == | TRUE if a has the same value as b           | a == b (TRUE)  |
| != | TRUE if a does not have the same value as b | a != b (FALSE) |
| >  | TRUE if a is greater than b                 | a > b (FALSE) |
| <  | TRUE if a is less than b                    | a < b (FALSE) |
| >= | TRUE if a is greater than or equal to b     | a >= b (TRUE) |
| <= | TRUE if a is less than or equal to b        | a <= b (TRUE) |

- These operators evaluate to TRUE or FALSE depending on the values you give them.
- Conditionals are used to instruct computer to make a decision.

## Examples

```r
45 > 34
45 > 79
45 < 79
45 < 34

23.1 >= 23
23.1 >= 23.1
23.1 <= 23.1
23.1 <= 23

67.3 == 87
67.3 == 67
67.0 == 67
67.0 != 67
67.0 != 23
```

##  Combining Comparisons

```r
x = 2
y = 5
z = 7
x < y && y < z


```