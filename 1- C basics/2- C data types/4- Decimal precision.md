By default after printing a float point number the output will show many digits after the decimal point to remove the extra zeros we can use a dot followed by a number that specifies how many digits that should be shown:
```
float myFloatNum = 3.5;  
  
printf("%f\n", myFloatNum);   // Default will show 6 digits after the decimal point  
printf("%.1f\n", myFloatNum); // Only show 1 digit  
printf("%.2f\n", myFloatNum); // Only show 2 digits  
printf("%.4f", myFloatNum);   // Only show 4 digits
```
