# Vectors

* Vectors allow you to store multiple values of the same data type. If you have mixed data types, then all the values will be converted to character data type.

## Create a new vector

```r
v = c(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
```

## Access an element

* Index is 1-based, meaning the first element is at index location 1

```r
v[1]
v[10]
```

```r
v[11]
```

* `NA` is another data type that indicates that you have a missing value.

## Selecting multiple elements

```r
v[1:5]
v[seq(1, 10, 2)]
```

## Built-in Vector Functions

* sum() Sum of all element values
* length() Number of elements
* unique() Generate vector of distinct values
* diff() Generate vector of first differences
* sort() Sort elements, omitting NAs
* order() Sort indices, with NAs last
* rev() Reverse the element order
* summary() Information about object contents

```r
y = c(1, NA, 3, 2, NA)
sum(y)
```

```r
y = c(1, NA, 3, 2, NA)
summary(y)
```

```r
y = c(1, NA, 3, 2, NA)
sum(y, na.rm=TRUE) 
```
