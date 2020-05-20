A[3] int

|   |   |
| --- | --- |
|   |     ```int -->  4 bytes``` |
|   |   |
|   |           4X3 = 12 bytes|
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |


|   |  200 | 204  |  208 |   |   |   |   |  300 | 304  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|   |  2 | 5  |  1 |   |   |   |   |  8 |   |

| int *p;  | p=&x  |  p=&A[0]  |
| --- | --- |--- |--- |--- |
| print p  |  address of x |  200  |
| print(*p) | 8 | 2 |
|  print(*p+1)   | random  |   5 |
| print(* (A+1)) | 5 |--- |--- |--- |
| print(*A + 1)) | 6 |--- |--- |--- |


| Element at i | --- | --- | --- | --- |
| --- | --- | --- | --- | --- |
| --- | Address | --> | &A[i]| (A+i) |
| --- | Value | --> | A[i] | *(A+i) |

```C
for(i=0; i< 3; i++){
    printf("%d\n", &A[i] ); //Address
    printf("%d\n", A[i] );  // Value
}

```

A is a  pointer to the base address 
int *p = A
pn++ increments the value of the pointer

[Multi-dimentional Arrays ](multidimarrays.md) 