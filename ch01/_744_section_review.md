## 1.
> Describe the ADC instruction.
```
The ADC (add with carry) works the same as the ADD instruction, with the added feature of also adding the value of the carry flag to the destination operand.
```

## 2.
> Describe the SBB instruction.
```
```

## 3.
> What will be the values of EDX:EAX after the following instructions execute?
```
mov edx, 10h
mov eax, 0A0000000h
add eax, 20000000h
adc edx, 0
```
```
EDX:EAX = 00000010C0000000h
```

## 4.
> What will be the values of EDX:EAX after the following instructions execute?
```
mov edx, 100h
mov eax, 80000000h
sub eax, 90000000h
sbb edx, 0
```
```
EDX:EAX = 
```

## 5.
> What will be the contents of DX after the following instructions execute (STC sets the Carry flag)?
```
mov dx, 5
stc
mov ax, 10h
adc dx, ax
```
```
DX = 0016h
```
