# Introduction to Functions

A Functions is a small, self-contained sequence of statements/instructions that has a name. Example: a function to convert Celsius to Fahrenheit. Since the formula for converting from Celsius to Fahrenheit is always the same and the only variable is the temperature in Celsius, you can write a function that takes the temperature as an argument, perform the conversion, and then return the temperature in Fahrenheit.

What are the advantages of using functions?

- Many programs require a particular sequence of statements/instructions to be executed repeatedly. The repeated statements/instructions can be placed with a single function, which can be accessed whenever needed. Therefore, they reduce repeated statements/instructions.
- Functions help decompose larger programs into logical subprograms. Such programs are easier to write and debug.
- Functions can be executed at any point by using their name
- Functions can call other functions
- Functions can OPTIONALLY take argument(s) that they can use inside the function
- Functions can OPTIONALLY return value(s)

The general form of a function call is as follows:

```r
<<function_name>> = function(<<parameters>>) {
    body
}
```

```{note}
Note the difference between parameters and arguments: Function parameters are the names listed in the function's definition. Function arguments are the real values passed to the function. Parameters are initialized to the values of the arguments supplied.  [Reference](https://developer.mozilla.org/en-US/docs/Glossary/Parameter)
```

## Built-in Functions

R comes with many useful functions.

seq(), mean(), max(), sum(x) and paste(...)

```r
seq(1, 10)
```

```r
sum(10, 20, 10)
```

```r
max(10, 20, 10)
````

```r
paste(3, .14)
```

```r
paste(3, '.14', sep='')
```

## User-defined Functions

```r
area_of_rectangle = function(length, width) {
    return (length * width)
}
```

Ref:[Formulas](https://www.austincc.edu/pintutor/pin_mh/_source/Handouts/Geometry_Formulas/Geometry_Formulas_2D_3D_Perimeter_Area_Volume.pdf)
