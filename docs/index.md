---
title: "Advanced Data Science for Planners"
subtitle: 'Excercise 1.Data Types in R Answer Keys'
author: "Fang Fang"
knit: (function(input_file, encoding) {
  out_dir <- 'docs';
  rmarkdown::render(input_file,
 encoding=encoding,
 output_file=file.path(dirname(input_file), out_dir, 'index.html'))})
output: 
  html_document: 
    keep_md: yes
    toc: true
---


### Question 1: 
Execute the commends below. What is the data type for x?

```r
x  <- 5
class(x)
```

Answer: Numeric


### Question 2: 
Execute the commands below. Is `y` an integer, logical or numeric data? 

```r
y <-5.0
is.integer(y)
is.numeric(y)
is.logical(y)
```

Answer: Numeric


### Question 3: 
Try out the commends below. What is the data type for `test2`? Numeric or character? 


```r
test2 <- "34.443"

class(test2)
```

Answer: Character. 

### Question 4:

What is the data type for `eva_scores` ? 
Answer: Logical

### Question 5:

Use the `matrix` function to generate the matrix below:

 Row number | first column  | Second column | Third column | Fourth column
------------- | -------------| -------------|-------------|-------------
1st row  | 10 |11|12|13
2nd row | 14 |15|16|17
3rd row |18|19|20|21

Answer: 


```r
m <- matrix(10:21, nrow=3, ncol=4, byrow=T)
```


### Question 6:

Try to use index numbers to extract the 3rd column from iris data instead of using `iris$Petal.Length`.

Answer: 


```r
iris[,3]
```



### Question 7: 

Try the command below to extract hour (it should be `8`) from `time_chr`. Does it work or not? Why?


```r
hour_example <- hour(time_chr)
```


Answer: It does not work since `time_chr` is character data type. 

### Question 8

Examine the data type of the first column in the `Beach_Water_Quality` data set. Convert it into a factor data type. What are the unique values for this column? 


```r
water$`Beach Name` <-  factor(water$`Beach Name`)
levels(water$`Beach Name`)
```

