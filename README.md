# Python/R conversion cheatsheet: How to do everything you do in Python in R and vice versa

<br>

### Variable assignment

#### R
```r
x <- 2    # x = 2 also works though it is bad form
```

#### Python 
```python
x = 2
```
<br>

### Exponentials

#### R
```r
2^3    #8
```

#### Python 
```python
2**3    #8
```
<br>

### Convert text to lowercase

#### R
```r
tolower("THIS is a STRING")
```

#### Python 
```python
"THIS is a STRING".lower()
```
<br>

### Convert text to uppercase

#### R
```r
toupper("THIS is a STRING")
```

#### Python 
```python
"THIS is a STRING".upper()
```
<br>

### Join two or more strings with spaces

#### R
```r
paste("join", "these", "strings", sep=" ")
```

#### Python 
```python
"join" + " " + "these" + " " + "strings"
```
<br>

### Remove leading or trailing whitespace from a string

#### R
```r
trimws("   example string    ")
```

#### Python 
```python
"   example string    ".strip()
```
<br>

### Convert numeric value to string

#### R
```r
as.character(3)
```

#### Python 
```python
str(3)
```
<br>

### Making a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
```
<br>

### Getting the length of a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
length(x)
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
len(x)
```
<br>

### Accessing the last element in a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
x[length(x)]
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x[-1]
```
<br>

### Modifying an element in a vector/array (R) or list (Python)

Note: indices start at 1 in R and 0 in Python

#### R
```r
x <- c(5, 2, 3, 1, 4)
x[1] <- 3    #3, 2, 3, 1, 4
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x[0] = 3    #3, 2, 3, 1, 4
```
<br>

### Appending an element to a vector/array (R) or list (Python)

Note: indices start at 1 in R and 0 in Python

#### R
```r
x <- c(5, 2, 3, 1, 4)
x <- c(x, 7)
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x.append(7)
```
<br>

### Removing an element in a vector/array (R) or list (Python)

Note: indices start at 1 in R and 0 in Python

#### R
```r
x <- c(5, 2, 3, 1, 4)
x <- x[-4]    #removes 1
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
del x[3]    #removes 1
```
<br>

### Sorting a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
x <- sort(x)
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x.sort()
```
<br>

### Reverse the order of a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
x <- rev(x)
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x.reverse()
```
<br>

### Making an empty vector/array (R) or list (Python)

#### R
```r
x <- NULL
```

#### Python 
```python
x = []
```
<br>

### Looping through a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
for(i in x){
    print(i)
}
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
for i in x:
    print(i)
```
<br>

### Making a continuous sequence of integers

#### R
```r
x <- 1:10    #also, seq(1, 10)
```

#### Python 
```python
x = range(1, 11)
```
<br>

### Making a non-continuous sequence of integers

#### R
```r
x <- seq(1, 11, 2)    #1, 3, 5, 7, 11
```

#### Python 
```python
range(1, 12, 2)    #1, 3, 5, 7, 11
```
<br>

### Squaring all elements in a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
x^2    #25, 4, 9, 1, 16
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
for i in x:
    print(i**2)    #25, 4, 9, 1, 16
```
<br>

### Cubing all elements in a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
x^3    #125, 8, 27, 1, 64
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
for i in x:
    print(i**3)    #125, 8, 27, 1, 64
```
<br>

### Suming all elements in a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
sum(x)    #15
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
sum(x)    #15
```
<br>

### Subsetting a vector/array (R) or list (Python)

#### Between two indices:

#### R
```r
x <- c(5, 2, 3, 1, 4)
x[2:4]    #2, 3, 1
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x[1:4]     #2, 3, 1
```
<br>

#### From the beginning to an index:

#### R
```r
x <- c(5, 2, 3, 1, 4)
x[1:4]    #5, 2, 3, 1
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x[ :4]     #5, 2, 3, 1
```
<br>

#### From an index to the end:

#### R
```r
x <- c(5, 2, 3, 1, 4)
x[2:length(x)]    #2, 3, 1, 4
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x[1:]     #2, 3, 1, 4
```
<br>

<br>

#### From the end to the end-n (e.g., n=2):

#### R
```r
x <- c(5, 2, 3, 1, 4)
x[(length(x)-2):length(x)]    #3, 1, 4
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
x[-3: ]     #3, 1, 4
```
<br>

### Making a (deep) copy of a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
y <- x
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
y = [:]
```
<br>

### Booleans

#### R
```r
TRUE
FALSE
```

#### Python 
```python
True
False
```
<br>


### If else statements

#### R
```r
x <- 1
if(x > 3){
    print("x > 3")
} else {
    print("x < 3")
}
```
#### alternatively:
```r
x <- 1
ifelse(x > 3, "x > 3", "x < 3")
```

#### Python 
```python
x <- 1
if x > 3:
    print("x > 3")
else:
    print("x < 3")
```
<br>

### If else-if else statements

#### R
```r
x <- 1
if(x > 3){
    print("x > 3")
} else if (x < 3)  {
    print("x < 3")
} else {
    print("x == 3")
}
```

#### Python 
```python
x = 1
if x > 3:
    print("x > 3")
elif x < 3:
    print("x < 3")
else:
    print("x == 3")
}
```
<br>

### Logical operators

#### Or:

#### R
```r
2 > 1 | 3 > 4    #TRUE
```

#### Python 
```python
2 > 1 or 3 > 4    #True
```
<br>

#### And:

#### R
```r
2 > 1 & 3 > 4    #FALSE
```

#### Python 
```python
2 > 1 & 3 > 4    #False
```
<br>

### Checking if a value is in a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
1 %in% x
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
1 in x
```
<br>

### Checking if a value is NOT in a vector/array (R) or list (Python)

#### R
```r
x <- c(5, 2, 3, 1, 4)
! 1 %in% x
```

#### Python 
```python
x = [5, 2, 3, 1, 4]
1 not in x
```
<br>

### Building a empty list (R) or Dictionary (Python)

#### R
```r
x <- list()
```

#### Python 
```python
x = {}
```
<br>

### Accessing elements in a list (R) or Dictionary (Python)

#### R
```r
x <- list(y = 2, z = c(1, 2, 3))
x[["y"]]
```

#### Python 
```python
x = {'y': 2, 'z': [1, 2, 3]}
x["y"]
```
<br>

### Building a list (R) or Dictionary (Python)

#### R
```r
x <- list(y = 2, z = c(1, 2, 3))
```

#### Python 
```python
x = {'y': 2, 'z': [1, 2, 3]}
```
<br>

### Accessing elements in a list (R) or Dictionary (Python)

#### R
```r
x <- list(y = 2, z = c(1, 2, 3))
x[["y"]]
```

#### Python 
```python
x = {'y': 2, 'z': [1, 2, 3]}
x["y"]
```
<br>

### Modifying elements in a list (R) or Dictionary (Python)

#### R
```r
x <- list(y = 2, z = c(1, 2, 3))
x[["z"]][1] <- 5    #z = 5, 2, 3
```

#### Python 
```python
x = {'y': 2, 'z': [1, 2, 3]}
x["z"][0] = 5    #z = 5, 2, 3
```
<br>

### Adding new elements in a list (R) or Dictionary (Python)

#### R
```r
x <- list(y = 2, z = c(1, 2, 3))
x[["w"]] <- 1    #or, x$w <- 1
```

#### Python 
```python
x = {'y': 2, 'z': [1, 2, 3]}
x["w"] = 1
```
<br>

### Removing elements in a list (R) or Dictionary (Python)

#### R
```r
x <- list(y = 2, z = c(1, 2, 3))
x[["z"]] <- NULL
```

#### Python 
```python
x = {'y': 2, 'z': [1, 2, 3]}
del x["z"]
```
<br>
