# BDA-practicals

## Practical 1: Write an R-Program to demonstrate working with Arithmetic operators.

## Code: 
```R
vect1 <- c(4,5,6)
vect2 <- c(7,8,9)
cat("addition of vector is", vect1+vect2)
cat("substraction of vector is", vect1-vect2)
cat("multiplication of vector is", vect1*vect2)
cat ("division of vector is", vect1/vect2)
cat ("modulus of vector is", vect1%%vect2)
```

## Practical 2: Write an R Program to Find the Factorial of a Number.

## Code:
```R
num <- -1
if(num < 0){
  cat("Factorial is not defined for negative numbers.\n")
} else if(num == 0 || num == 1){
  cat("Factorial is 1\n")
} else {
  res <- 1
  for(i in 2:num){
    res <- res * i
  }
  cat("Factorial is", res, "\n")
}
```

## Practical 4: Write an R Program to create a Matrix and access rows and columns using functions colnames() and rownames() .

## Code:
```R
a = matrix(c(11,12,13,14,15,16,17,18,19),3,3,byrow=TRUE)
rownames(a)<-letters[1:3]
print(a)

b = matrix(c(21,22,23,24,25,26,27,28,29),3,3,byrow=TRUE)
colnames(b)<-letters[1:3]
print(b)
```

## Practical 5: Write an R Program to create a List and modify its components. 

## Code: 
```R
lt = list( 
 a=10, 
 char_vector=letters[1:4], 
 mat1=matrix(c(1,2,3,4,5,6), nrow = 2), 
 mat2=matrix(1:6, nrow = 3) 
) 
print("list before modificaiton:\n") 
print(lt) 
lt$a=20 
print("list after modification:\n") 
print(lt)
```

## Practical 6: Write an R Program to create a Matrix from a Vector using dim() function. 

## Code:
```R
mat <- c(32,12,53,41,64,23,74,28) 
dim(mat) <- c(4,2) 
print(mat)
```

## Practical 7: Write an R Program to create a List and modify its components. 

## Code: 
```R
lt = list( 
 a=10, 
 char_vector=letters[1:4], 
 mat1=matrix(c(1,2,3,4,5,6), nrow = 2), 
 mat2=matrix(1:6, nrow = 3) 
) 
print("list before modificaiton:\n") 
print(lt) 
lt$a=20 
print("list after modification:\n") 
print(lt)
```