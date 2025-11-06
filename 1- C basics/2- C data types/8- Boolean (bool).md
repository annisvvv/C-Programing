Boolean data type are either true or false, this data type is not build in so it is necessary to import the following header file :
```
#include <stdbool.h>
```

A Boolean variable is declared with the `bool` keyword :
```
bool isProgrammingFun = true;  
bool isFishTasty = false;
```

Boolean return as integers 1 for true and 0 for false therefor the `%d` format specifier must be used to print a Boolean value.

It is more common to return Boolean value by comparing values and variables.
# Comparing values and variables
Using comparison operators :
```
printf("%d", 10 > 9);  // Returns 1 (true) because 10 is greater than 9

///////////////////////////////////////////
int x = 10;  
int y = 9;  
printf("%d", x > y);

///////////////////////////////////////////
printf("%d", 10 == 10); // Returns 1 (true), because 10 is equal to 10  
printf("%d", 10 == 15); // Returns 0 (false), because 10 is not equal to 15  
printf("%d", 5 == 55);  // Returns 0 (false) because 5 is not equal to 55

///////////////////////////////////////////
bool isHamburgerTasty = true;  
bool isPizzaTasty = true;  
  
// Find out if both hamburger and pizza is tasty  
printf("%d", isHamburgerTasty == isPizzaTasty);
```