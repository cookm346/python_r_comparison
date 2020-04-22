# Python/R conversion cheatsheet: How to do everything you do in Python in R and vice verse

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