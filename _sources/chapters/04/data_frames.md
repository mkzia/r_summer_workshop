# DataFrames

DataFrame is a table or a 2D array with rows and columns.

```r
student_ids = c(111, 222, 333)
names = c('John', 'Jane', 'Jack')
grades = c(70, 89, 85)

student_info = data.frame(
    id = student_ids,
    name = names,
    grade = grades
)
```

## Select a single column by name

```r
student_info['id']
student_info['name']
```

## Select a multiple columns by name

```r
student_info[c('id', 'name')]
```

## Select a single column by index

* [ROW, COLUMN]

```r
student_info[,1]
student_info[,2]
```

## Select a multiple columns by index

* [ROW, COLUMN]

```r
student_info[,c(1, 2)]
```

## Select a single row, all columns

```r
student_info[1,]
```

## Select a single row, some columns

```r
student_info[1,c(1, 2)]
```

## Select a single row, some columns

```r
student_info[1,c(1, 2)]
student_info[1,c('id', 'name')]
```

## Select multiple rows by range, some columns

```r
student_info[1:2,c(1, 3)]
```

## Select multiple rows by index, some columns

```r
student_info[c(1, 3),c(1, 3)]
```

## Read TSV file

```r
df = read.csv('students.tsv', sep='\t')
```

## Select All Melissas

```r
df[df['First'] == 'Melissa']
```

## Add average column

```r
df['Average'] = round((df$Exam1 + df$Exam2 + df$Exam3)/3)
```

## Get Max Average

```r
df[which.max(df$Average), ]
```

## Get Min Average

```r
df[which.max(df$Average), ]
```

## Order column

```r
df[order(df$Average)]
```

## Select all grades >=70

```r
gte70 = df[df$Average>=70,]
```

## Load SEPA Data

```
df = read.csv('SEPA-2023-Metadata.csv')
```

## Split GPS data

```r
Value = df[df$Metadata == 'GPS', 'Value']
temp = str_split_fixed(Value, ', ', 2)
Latitude = as.numeric(temp[,1])
Longitude= as.numeric(temp[,2])
GPS = df[df$Metadata == 'GPS', ]
GPS['Latitude'] = Latitude
GPS['Longitude'] = Longitude
```

## Combine Value with Unit

```r
df['Combined'] = paste(df[,'Value'], df[,'Unit'])
df$Combined = paste(df$Value, df$Unit)
```
