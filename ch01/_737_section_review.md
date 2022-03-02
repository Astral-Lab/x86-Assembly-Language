## 1.
> Explain why overflow cannot occur when the MUL and one-operand IMUL instructions execute.

```
The greatest product of the multiplicand and multiplier will always be less than what the destination can store.
This can be proven by mathematical induction.
```

## 2.
> How is the one-operand IMUL instruction different from the MUL in the way it generates a multiplication product?

```
IMUL retains the sign of the product.
```

## 3.
> What has to happen in order for the one-operand IMUL to set the Carry and Overflow flags?

```
If the upper half of the product is not a sign extension of the sign bit of the lower half, then the overflow and carry flags will be set.
```

## 4.
> When EBX is the operand in a DIV instruction, which register holds the quotient?

```
EAX.
```

## 5. 
> When BX is the operand in a DIV instruction, which register holds the quotient?

```
AL.
```

## 6.
> When BL is the operand in a MUL instruction, which registers hold the product?

```
AX.
```

## 7.
> Show an example of sign extension before calling the IDIV instruction with a 16-bit operand.

```
mov ax, 8000h
cwd
mov bl, 2
idiv bl
```
