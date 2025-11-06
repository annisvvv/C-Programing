 we can get the **memory address** of a variable with the reference operator `&`:

```
int myAge = 43; // an int variable  
  
printf("%d", myAge);  // Outputs the value of myAge (43)  
printf("%p", &myAge); // Outputs the memory address of myAge (0x7ffe5367e044)
```

A **pointer** is a variable that **stores** the **memory address** of another variable as its value.

A **pointer variable** **points** to a **data type** (like `int`) of the same type, and is created with the `*` operator.

The address of the variable you are working with is assigned to the pointer:

```
int myAge = 43;     // An int variable  
**int* ptr = &myAge;**  // A pointer variable, with the name ptr, that stores the address of myAge  
  
// Output the value of myAge (43)  
printf("%d\n", myAge);  
  
// Output the memory address of myAge (0x7ffe5367e044)  
printf("%p\n", &myAge);  
  
// Output the memory address of myAge with the pointer (0x7ffe5367e044)  
printf("%p\n", ptr);
```

Create a pointer variable with the name `ptr`, that **points to** an `int` variable (`myAge`). Note that the type of the pointer has to match the type of the variable you're working with (`int` in our example).

Use the `&` operator to store the memory address of the `myAge` variable, and assign it to the pointer.

Now, `ptr` holds the value of `myAge`'s memory address.
# Dereference
In the example above, we used the pointer variable to get the memory address of a variable (used together with the `&` **reference** operator).

You can also get the value of the variable the pointer points to, by using the `*` operator (the **dereference** operator):
```
int myAge = 43;     // Variable declaration  
int* ptr = &myAge;  // Pointer declaration  
  
// Reference: Output the memory address of myAge with the pointer (0x7ffe5367e044)  
printf("%p\n", ptr);  
  
// Dereference: Output the value of myAge with the pointer (43)  
printf("%d\n", *ptr);
```

Note that the `*` sign can be confusing here, as it does two different things in our code:

- When used in declaration (`int* ptr`), it creates a **pointer variable**.
- When not used in declaration, it act as a **dereference operator**.
```
int* myNum;  
int *myNum;
```