1. The bug was that there is an error in the declaration of num1 and num2.
   Both of them are declared as string and hence the + operator is concatinating them.

2. To fix the error, we can use `ParseInt()` method on num1 and num2 to convert them to Integer values