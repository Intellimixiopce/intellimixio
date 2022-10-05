## Dynamic Memory Allocation in C

- In this article, we will discuss how memory can be allocated dynamically in the C programming language.

### Introduction

>  Memory that has been allocated at compilation time cannot be altered after execution. This will result in a problem with memory loss or inadequacy.
>
> -  The answer is to dynamically create memory, that is, according to user requirements as the programme is being run.
>- There are two ways to allocate memory:
>  > 1. static Memory Allocation
>  > 2. Dynamic Memory Allocation

The standard library functions used for dynamic memory management are:
 

 - Malloc()
 - Calloc()
 - Realloc()
 - Free()
 ## Malloc()
 - Using this function, a runtime byte-sized memory block can be allocated.
 - It gives back a void pointer that points to the base address of the memory that was allocated.
 - Unknown values will be present in the allotted RAM because it has not been initialised.

 **Syntax:**
```
void *malloc (size in bytes);
```
## Calloc()
 - This function is utilized to allocate continuous memory chunks during runtime.
- This was created specifically for arrays.
- It gives back a void pointer that points to the base address of the memory that was allocated.


**Syntax:**
```
 void *calloc ( numbers of elements, size in bytes);
```
## Realloc()
 - It can reduce (or) extend the allocated memory and reallocates previously allocated memory. 
 - It then returns a void pointer that points to the base address of the newly allocated memory.
 **Syntax:**
```
void *realloc (pointer, newsize);
```
## Free()
 - With dynamic runtime allocation, it is our obligation to release the space when it is not needed for efficient memory consumption. 
 - This function frees (or) dealslocates previously allocated memory space.
  **Syntax:**
```
void *free (pointer);
```


**program to demonstrate  standard library functions used for dynamic memory management.**
```
#include<stdio.h>

void main()

{

int *arr,i,j,n;

clrscr();

printf("enter the number of elements in array");

scanf("%d",&n);

arr=(int*) malloc(n*sizeof(int));  //dynamically allocating memory

//code to read the elements of an array

for(i=0;i<n;i++)

{

printf("enter %d elment",i+1);

scanf("%d",&arr[i]);

}

//code to display elements of array

printf("elements in array are");

for(i=0;i<n;i++)

printf(" \t %d",arr[i]);

//code to increase the size of an array by  using realloc function

arr=(int*)realloc(arr, n+2);

arr[n]=9;

arr[n+1]=10;

printf("element of an array after reallocating memory");

for(i=0;i<=n+1;i++)

printf("\t %d",arr[i]);

free(arr);

getch();

return;

}
```
**Output:**

enter the number of elements in array 3

0  1  2

enter 1 element 10

enter 2 element 20

enter 3 element 30

elements in array are

10  20  30

element of an array after reallocating memory

10  20  30  9  10