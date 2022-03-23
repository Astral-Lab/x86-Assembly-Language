## 1.
> (True/False): A subroutine's stack frame always contains the caller's return address and the subroutine's local variables.

```
True. A stack frame consists of a subroutines arguments, return address, local variables, and saved registers.
```

## 2.
> (True/False): Arrays are passed by reference to avoid copying them onto the stack.

```
True. If we were to copy them onto the stack, then it would add a lot of code clutter, execute slowly, and use up stack space.
```

## 3.
> (True/False): A subroutine's prolouge code always pushed EBP on the stack.

```
True.
```

## 4.
> (True/False): Local variables are created by adding a positive value to the stack pointer.

```
False. When pushing an element onto the runtime stack, the ESP pointer is decremented. Hence, local variables 
are created by subtracting the stack pointer, not adding a positive value to it.
```

## 5.
> (True/False): In 32-bit mode, the last argument to be pushed on the stack in a subroutine call is stored at location EBP + 8.

```
```

## 6.
> (True/False): Passing by reference means that an argument's address is stored on the run-time stack.

```
True.
```

## 7.
> What are the two common types of stack parameters?

```
Value parameters and reference parameters.
```
