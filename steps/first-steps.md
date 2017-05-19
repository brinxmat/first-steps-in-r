# First Steps in R

## Hello world

```
print("Hello, World!")
```
>[1] "Hello, World!"

## Variable assignment

```
myString <- "Hello, World!"
print(myString)
```
>[1] "Hello, World!"

## Datatypes

```
myString <- "Hello, World!"
class(myString)
```
> [1] "character"

```
class('Hallo!')
```
> [1] "character"

```
myNumber <- 1
class(myNumber)
```
> [1] "numeric"

```
myNumber <- 1.778
class(myNumber)
```
> [1] "numeric"

```
myNumber <- 1L
class(myNumber)
```
> [1] "integer"

```
myNumber <- 1.778L
```
> Warning message:
> integer literal 1.778L contains decimal; using numeric value 

```
class(myNumber)
```
> [1] "numeric"

```
myBool <- TRUE
class(myBool)
```
>[1] "logical"

```
myComplexNumber <- 2 + 3i
class(myComplexNumber)
```
> [1] "complex"

```
myRaw <- charToRaw("Hello, World!")
myRaw
```
> [1] 48 65 6c 6c 6f 2c 20 57 6f 72 6c 64 21

```
class(myRaw)
```
> [1] "raw"

**Note:**

```
myString <- "This is a string"
class(myString)
```
> [1] "character"

```
typeof(myString)
```
> [1] "character"
 
```
storage.mode(myString)
```
> [1] "character"

```
myNumeric <- 1.8
class(myNumeric)
```
> [1] "numeric"
 
```
typeof(myNumeric)
```

> [1] "double"

```
storage.mode(myNumeric)
```

> [1] "double"

```
myInteger <- 2L
typeof(myInteger)
```
> [1] "integer"

```
storage.mode(myInteger)
```
> [1] "integer"


## Data structures

### Vectors

#### Atomic vectors

```
myAtomicVector <- vector() # empty vector

myAtomicVector <- vector(length = 10) # empty vector with size

# vectors for types with size
# vectors are only applicable for character, numeric, integer, logical

myAtomicVector <- vector("character", length = 10)
myAtomicVector <- vector("numeric", length = 10)
myAtomicVector <- vector("integer", length = 10)
myAtomicVector <- vector("logical", length = 10)

# assigning data

myCharacterVector <- c("in", "case", "of", "laughter")
myNumericVector <- c(1, 1.2, 1.8, 2.1)
myIntVector <- c(1L, 2L, 3L, 4L)
myLogicalVector <- c(TRUE, FALSE, FALSE, FALSE)
```

```
# inspecting vectors
typeof(myCharacterVector)
```
> [1] "character"

```
length(myCharacterVector)
```
> [1] 4

```
class(myCharacterVector)
```
> [1] "character"

```
str(myCharacterVector)
```

> chr [1:4] "in" "case" "of" "laughter"

```
typeof(myNumericVector)
``` 

> [1] "double"

```
length(myNumericVector)
``` 

> [1] 4

```
class(myNumericVector)
``` 

> [1] "numeric"

```
str(myNumericVector)
``` 
> num [1:4] 1 1.2 1.8 2.1

```
typeof(myIntVector)
``` 
> [1] "integer"

```
length(myIntVector)
```
> [1] 4

```
class(myIntVector)
```
> [1] "integer"

```
str(myIntVector)
```
> int [1:4] 1 2 3 4

```
typeof(myLogicalVector)

``` 
> [1] "logical"

```
length(myLogicalVector)

``` 

> [1] 4

```
class(myLogicalVector)

``` 

> [1] "logical"

```
str(myLogicalVector)
``` 

> logi [1:4] TRUE FALSE FALSE FALSE

```
# add items
myCharacterVector <- c(myCharacterVector, "break", "glass")
str(myCharacterVector)
```
>  chr [1:6] "in" "case" "of" "laughter" "break" "glass"



