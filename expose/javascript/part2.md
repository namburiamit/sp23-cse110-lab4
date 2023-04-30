# Part 2

1. The output is 3.
   * The value of i at the end of loop interations is 3 as there are 3 elements in the array.
  
   * The the keyword _var_ is used, 'i' has function scope and not block scope and hence it does not return an error and gives 3 as output.

2. The output is 150.
   * In the last iteration of the for loop, the discountedPrice variable was equal to `prices[2] * (1- 0.5)` which is 300 * 0.5 = 150.
  
   * Since the keyword _var_ is used to define the variable, it has function scope and we can access it. Hence, it stores the value 150.

3. The output is 150.

   * In the last iteration of the for loop, the discountedPrice = 150 (from 2).
  
   * `finalPrice = Math.round(discountedPrice * 100)/100` which (150*100)/100 = 150.
  

   * Since the keyword _var_ is used to define the variable, it has function scope and we can access it. Hence, it stores the value 150.

4. The function will return an array **[50, 100, 150]** 
   * All the values in the original array will be halved as the discount is 0.5.
   * Since the keyword _var_ is used to define the variable _'discounted'_, it has function scope and we can access it. Hence it stores an array [50, 100, 150].


5. ERROR
   * There is an error accessing variable _'i'_ as the keyword **let** was used to define the variable which has bock scope (for loop in this case).
   *   Hence, it's an error as line 12 can't access 'i'.
  
6. ERROR
   * There is an error accessing variable _'discountedPrice'_ as the keyword **let** was used to define the variable which has bock scope (for loop in this case).
   * Hence, it's an error as line 13 can't access 'discountedPrice'.

7. The output is 150.
   * In the last iteration of the for loop, the discountedPrice = 150 (from 2).
   * `finalPrice = Math.round(discountedPrice * 100)/100` which (150*100)/100 = 150.
   * Although _'let'_ variable was used to declare the variable, it was defined in the same scope as it was printed out (funciton scope in this case).
   * Hence, there is no error and the output is 150.

8. The function will return an array **[50, 100, 150]** 
    * All the values in the original array will be halved as the discount is 0.5.
   * Although _'let'_ variable was used to declare the variable, it was defined in the same scope as it was printed out (funciton scope in this case).
   * Hence, there is no error and the output an array **[50, 100, 150]** 

9. ERROR
    * The variable _'i'_ is defined with the keyword **let** which has block scope (loop in this case).
    * Hence there is an error in line 11 as we can't access variable _'i'_

10. The output is 3.
    * The input array has length 3 and hence `const length = prices.length` stores 3.
    * Since it's a constant, we can't change the value again and hence the output is 3.
 
11. The output is [50, 100, 150]
    * All the values in the original array will be halved as the discount is 0.5.
    * Although `discounted[]` was defined as a constant, we are not updating any existing value but just adding elements to the array.
    * Hence, there is no error and the output is [50, 100, 150].

12. 
- A: student.name
- B: student["Grad Year"]
- C: student.greeting()
- D: student["Favorite Teacher"].name
- E: student.courseLoad[0]

13. 
- A: '32'
  - ‘3’ + 2 
  - It is 32 as + is a concat operator on strings and as 2 is not a string it will be converted to '2' and added to '3' which gives '32'.
- B: 1
  - ‘3’ - 2
  - Since - is not a string operator, '3' is converted to 3 and is subtracted by 2 which gives output as 1.
- C: 3
  - 3 + null
  - first operand/ 3 is an integer and hence null is converted to integer which will be 0. Hence 3+0 = 3.
- D: 3null
  - '3' + null
  - Since '3' is a string, null is converted to a string and '3' concat 'null' would be '3null'.
- E: 4
  - true + 3
    - Since 3 can't be a boolean true is converted to integer which is 1. Hence 1+3 = 4.
- F: 0
  - false + null
  - Since a + operator is used, they are converted to integers and 0+0 = 0.
- G: '3undefined'
  - '3' + undefined
  - Since + is  a string operator, undefined is converted to 'undefined' and is added to 3 which gives output as '3undefined'.
- H: NaN
  - '3' - undefined
  - Since string does not

14.  
- A: True
  - '2' converts to 2 and 2>1 is True.
- B: False
  - '2' < '12' is false as '12' is lexicographically smaller.
- C: True
  - 2 == '2' as the integer values of both are same. ('2' is converted to 2) (== equality check)
- D: False
  - 2 === '2' is false as **===** does equality as well as type check. It's false as numeric value ≠ string value.
- E: False
  - True(1) ≠ 1. Hence, false.
- F: True
  - Boolean(2) = true
  - Since both are boolean values and are equal, the condition is satisfied. Hence, it's true.

15.  
    * The **==** operator checks if the Left hand and Right hand values are equal without checking the type of the values.

    * The **===** operator checks if the Left hand and Right hand values are equal along with checking the type of both the values. Returns true iff both value and type are equal.

16.  Refer to **part2-question16.js**

17.  The output is an array [2, 4, 6]
    * The _modifyArray_ function takes in an array and callback funciton as parameters and then while pushing elements to newArr, the callback funciton is used (in this case doSomething). 
    * 'doSomething' essentially takes in the element and doubles it. 
    * Hence while adding everytime, the element's value is doubled and [1, 2, 3] turns into [2, 4, 6]
    * Hence, the output is [2, 4, 6]
  
18.   Refer to **part2-question18.js**

19.  The output is: 1 4 3 2