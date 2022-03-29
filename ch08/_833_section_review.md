## 1. 
> (True/False): Given the same task to accomplish, a recursive subroutine usually uses less memory than a nonrecursive one.

```
False.
```

## 2.
> In the Factorial function, what condition terminates the recursion?

```
cmp eax, 0
```

## 3.
> Which instructions in the assembly language Factorial procedure execute after each recursive call has finished?

```
mov ebx, [ebp+8]
mul ebx
pop ebp 
ret 4
```

## 4.
> What would happen to the Factorial program's output if you tried to calculate 13!?

```

```

## 5.
> Challenge: How many bytes of stack space would be used by the Factorial procedure when calculating 5!?

```
Bytes per stack frame = 12,
Number of frames = 6,
Total bytes = 12 x 6 = 72
```
