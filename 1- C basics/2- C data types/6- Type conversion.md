We sometimes need to convert the value of one data type to another. 

There is two types of conversion in C :
- **Implicit Conversion** (automatically)  
- **Explicit Conversion** (manually)
# Implicit Conversion
This is done automatically by the compiler when a value of one data type is assigned to another.

for example storing a int in a float will result to a float so storing 9 as a float will result to storing 9.000000 and the opposite is right.

As for another example dividing two integer will result to an integer so 5 / 2 is normally equal to 2.5 but storing them in a form of int will result to a int 2
```
int x = 5;  
int y = 2;
float sum = 5 / 2;  
  
printf("%f", sum); // 2.000000
```
# Explicit Conversion
This is done manually by placing the type in parentheses () in front of the value.
```
// Manual conversion: int to float  
float sum = (float) 5 / 2;  
  
printf("%f", sum); // 2.500000
```

```
int num1 = 5;  
int num2 = 2;  
float sum = (float) num1 / num2;  
  
printf("%f", sum); // 2.500000
```

```
int num1 = 5;  
int num2 = 2;  
float sum = (float) num1 / num2;  
  
printf("%.1f", sum); // 2.5
```
