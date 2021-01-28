1. i will be printed because it was defined as an "old school"
   variable, meaning that it has no block scope, only the function
   scope.

2. discounted will be printed because it was defined as an "old 
   school" variable, meaning that it has no block scope, only the function scope.

3. finalPrice will be printed because it was defined as an "old school"
   variable, meaning that it has no block scope, only the function
   scope.

4. The function will return the array [50, 100, 150] because the 
   function takes the discount off of each price in the input array

5. an error will be thrown because i is not defined. This is because
   i was initialized with `let` meaning that it adheres to block
   scope.

6. an error will be thrown because discountedPrice was defined with
   `let` in the for loop, meaning that it is out of the scope of line
   12

7. finalPrice will be printing because while finalPrice was 
   initialized with `let`, it is still in the same block scope as line
   13

8. The function will still return the array [50, 100, 150] because 
   the function takes the discount off of each price in the input 
   array

9. This line will not even run because the compiler will throw an 
   error at line 7 because the function is trying to change the value of finalPrice to something else, but it was defined earlier in line
   3 as a constant variable.

10. see 9
11. see 9
12. Nothing will be returned because the compiler will throw an 
    error at line 7 because the function is trying to change the
    value of finalPrice to something else, but it was defined earlier 
    in line 3 as a constant variable.

13. Notations
    1. student.name
    2. student['Grad Year']
    3. student.greeting()
    4. student['Favorite Teacher'].name
    5. student.courseLoad[0]

14. Arithmetic
    1. `'32'` - The statement outputted a string because it saw an
       addition sign and a string, thus it converted the 2 to a
       string and did string concatenation
    2. `1` - Since we're doing a minus operation, which is mainly for
       numerical subtraction, we convert the `'3'` to an integer and
       perform subtraction, getting 1
    3. `3` - Addition with an integer and null means that null will
       be converted to an integer, which is defined as 0. Thus, 
       3 + 0 = 3
    4. `3null` - Addition with a string and null means string
       concatenation. Thus null become the string 'null' and the
       two strings are concatenated.
    5. `4` - Addition with an integer and true means that true will
       be converted to an number, which is defined as 1. Thus, 
       3 + 1 = 4.
    6. `0` - It's a bit ambiguious what false + null should be. In
       this case JS defaults to numerical addition, and thus converts false to 0 and null to 0, resulting in 0 as the output.
    7. `3undefined` - Addition with a string and undefined means 
       string concatenation. Thus undefined become the string 
       'undefined' and the two strings are concatenated.
    8. `NaN` - Since we're doing a minus operation, which is mainly 
       numerical, we convert the string and undefined to numbers,
       which results in 3 and NaN. Since subtraction with NaN 
       doesn't make sense, JS returns NaN

15. Comparison
    1. `true` - Since there is one number in the comparision, JS will
       do numerical comparison and convert '3' to 3, then compute `2 > 1`
    2. `false` - Since there are two strings in the comparison, JS
       will perform string comparison. Since the ascii value of '2' is greater than '1' (first char in string '12'), this
       returns false.
    3. `true` - Since there is one number, JS will do numerical 
       comparison and convert '2' to 2, then compute `2 == 2` which
       is true
    4. `false` - Both sides of this comparison are different types,
       so the comparison will automatically return false
    5. `false` - Since there is one number, JS will do numerical 
       comparison and convert true to 1, then compute `1 == 2` which
       is false
    6. `true` - Before the comparison, Boolean(2) is processed. Since
       the input value is not any one of the values that output false
       (0, null, undefined, NaN, ""), Boolean(2) returns true. Now we
       compare `true === true`. Since they are equivalent and share the same type, this comparison evaluates to true.

16. `==` does equality comparison with type conversion, `===` does type conversion without type conversion.

17. `How are you?` will get printed. The first if statement check if `2 == true`. true will get converted to 1, then the if statement evaluates `2 == 1` which is false. JS moves on to the next statement, `else if (2)`. This is checking the boolean value of 2, which is true. Thus the program prints out `How are you?`.

19. The following array will be returned: `[6,8,10]`. First, we have a for loop that calls doSomething for each element in the array along with another nameless callback function that multipies its input by 2. doSomething inputs the input number plus 2 into the input callback function. Thus for each value in the array, values are processed as follows:
    
    array[0]: 1 -> 3 -> 6
    array[1]: 2 -> 4 -> 8
    array[2]: 3 -> 5 -> 10

These values get inserted into a new array which is returned.

21. Here's the output:
```
1
4
3
2
```