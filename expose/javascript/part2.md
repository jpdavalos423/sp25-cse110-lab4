1. Line 12 prints out 3. This is because it prints out the variable i which is meant to iterate through the prices arguments. Since only 3 arguments are passed in, once the counter reaches 3 the loop terminates but counter i remains active since it was declared as var in function scope.
2. Line 13 prints out 150. This is because it prints out the last discounted price which was .5 of 300 which is 150. Since the variable was declared as var, it remains active even after the for loop terminates as it is in function scope.
3. Line 14 prints out 150. This is because it was the last value that was pushed to discounted which is meant to keep track of all the discounted prices. 
4. The function will return all the prices passed in discounted by the discount rate passed in. In this case, the prices passed in were 100, 200, and 300 with a discount rate of .5 so the function will return 50, 100, 150.
5. At line 12, the function will throw an error that i is not defined when trying to print the value of i. This is expected as i was declared with let as a counter for the for loop and no longer exists after the loop terminates as it is block scoped.
6. At line 13, the function will throw an error that discountedPrice is not defined when trying to print the value of discountedPrice. This is expected as discountedPrice was declared with let in the for loop and no longer exists after the loop terminates as it is block scoped.
7. Line 14 prints out 150. This is because the variable finalPrice was declared with let in the same block as the function as is accessible outside of the for loop unlike i and discountedPrice.
8. The function will return all the prices passed in discounted by the discount rate passed in. In this case, the prices passed in were 100, 200, and 300 with a discount rate of .5 so the function will return 50, 100, 150.
9. At line 11, the function will throw an error that i is not defined when trying to print the value of i. This is expected as i was declared with let as a counter for the for loop and no longer exists after the loop terminates as it is block scoped.
10. Line 12 prints 3. This is because is prints length which contains the length of the prices argument which is 3.
11. The function will return all the prices passed in discounted by the discount rate passed in. In this case, the prices passed in were 100, 200, and 300 with a discount rate of .5 so the function will return 50, 100, 150.
12a. student.name;
12b. student["Grad Year"];
12c. student.greeting();
12d. student["Favorite Teacher"].name;
12e. student.courseLoad[0];
13a. 32, performed string concatnation
13b. 1, performed arithmetic, type casted "3" to 3
13c. 3, performed arithmetic, type casted null to 0
13d. 3null, performed string concatnation
13e. 4, performed arithmetic, type casted true to 1
13f. 0, performed arithmetic, type casted null and false to 0
13g. 3undefined, performed string concatnation
13h. NaN, performed arithmetic, type casted "3" to 3, and type casted undefined to NaN. Arithmetic with NaN always results in NaN
14a. true, '2' type casts to integer 2 and 2 is greater than 1.
14b. false, when comparing strings '2' and '12', 2 is lexicographically larger than 1 so this statement is false 
14c. true, '2' type casts to integer 2 and 2 is equal to 2 so the statement is true
14d. false, === does not type cast and since '2' is not the same as 2 the statement is false 
14e. false, true type casts to integer 1 which is not equal to 2 so the statement is false
14f. true, Boolean casting 2 results in true so the statement is true
15. == means loose equality so it converts both operands to the same type before comparing. === means strict equality so both operands must also be of the same type when comparing.
17. If the function modifyArray is called with parameters [1, 2, 3] and the doSomething function, it will double each value in the array resulting in the new array [2, 4, 6]. When modifyArray is called, a new array is made and the array passed in is iterated over. The doSomething function is called on the first value of the array which is 1 which returns 1 * 2 which is 2. This value is then pushed onto the new array. The next value 2 repeats the same process pushing the value 4 and the final value 3 results in pushing the value 6. This final array [2, 4, 6] is then returned giving us our final result. 
19. 1 4 3 2