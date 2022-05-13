## 1.
> Declare a MyStruct variable with default values.

```
struct1 MyStruct <>
```

## 2.
> Declare a MyStruct variable that initializes the first field to zero.

```
struct2 MyStruct <0,>
```

## 3.
> Declare a MyStruct variable and initialize the second field to an array containing all zeros.

```
struct3 MyStruct <, 20 DUP(0)>
```

## 4.
> Declare a variable as an array of 20 MyStruct objects.

```
struct4 MyStruct 20 DUP(<>)
```

## 5.
> Using the MyStruct array from the preceding exercise, move field1 of the first array
> element to AX.

```
mov ax, struct4[esi].field1
```

## 6.
> Using the MyStruct array from the preceding exercise, use ESI to index to the third array
> element and move AX to field1. Hint: Use the PTR operator.

```
mov esi, OFFSET struct4
add esi, 3 * (TYPE MyStruct)
mov (MyStruct PTR [esi]).field1, ax
```

## 7.
> What value does the expression TYPE MyStruct return?

```
WORD = 2 bytes, 
DWORD 20 DUP(?) = 80 bytes,

Answer: 82
```

## 8.
> What value does the expression SIZEOF MyStruct return?

```
SIZEOF and TYPE both return the same value when used with STRUCTs.

Answer: 82
```

## 9.
> Write an expression that returns the number of bytes in field2 of MyStruct.

```
mov eax, SIZEOF MyStruct.field2
```
