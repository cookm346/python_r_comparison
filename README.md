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
