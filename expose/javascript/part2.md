1. 3, It prints the length of the argument prices (or the final value of i after the for loop finishes). This is because even though the variable i is outside of the for loop/block, it was declared with var and that makes it ignore the loop/block and thus is still accessible from the outside of it. 

2. 150, because finalPrice is updated in each iteration of the loop using Math.round(discountedPrice * 100) / 100. Since it is declared outside the loop, it is accessible after the loop is done and ends up storing the value from the last iteration, which is 150.

3. 150, It prints the finalPrice for the last price in prices because in the for loop the variable finalPrice keeps getting reassigned by Math.round(discountedPrice * 100) / 100 of the ith price. Again, even though the finalPrice variable is outside of the for loop, it is still accessible within in it! 

4. [ 50, 100, 150 ], The function iterates through the prices, applies the discount, and stores the results in an array that is returned. Since var is function scoped, the loop variables remain accessible even after the loop completes.

5. ReferenceError: i is not defined. Error is returned because i was declared inside a for loop. Declaring it with let keeps the variable bounded to the loop’s block scope, so it is not accessible outside.

6. ReferenceError: discountedPrice is not defined. Error is returned because discountedPrice was declared inside the for loop block. Declaring it with let keeps the variable bounded to the loop’s block scope, so it is not accessible outside of it.

7. 150, because it the variable finalPrice was declared outside of any blocks, and thus is accessible. It specifically returns the last finalPrice value when the for loop is done.

8. [50, 100, 150], because finalPrice is updated each iteration and pushed into the discounted array. Since both are declared outside the loop with let, they are accessible inside it, so no error occurs.

9. TypeError: Assignment to constant variable. Because the for loop attempts to assign a value to the finalPrice variable (which was declared with const).

10. 3, which is weird because I thought it would've errored out with the const variables seemingly being changed. But upon further research, the program doesn’t error because each iteration of the loop creates a new block scope, so discountedPrice is a new const variable each time. Since const only prevents reassignment within the same scope, declaring it inside the loop is valid. discounted is not being reassigned and it still points to the same array. 

11. [50, 100, 150], [50, 100, 150], because the loop goes through each price, calculates price * (1 - discount), and pushes the result into the discounted array. There is no error since discounted and length are declared outside the loop and are accessible inside it, while i and discountedPrice are block-scoped and only used within the loop.

12.  
- A. student.name  
- B. student["Grad Year"]  
- C. student.greeting()  
- D. student["Favorite Teacher"].name  
- E. student.courseLoad[0]  

13.  
- A. 32, + with a string will be a concatenation  
- B. 1, - forces a '3' to be a numeric type = numeric conversion  
- C. 3, null = 0  
- D. 3null, + with a string will be a concatenation  
- E. 4, true = 1 so 1 + 3 = 4  
- F. 0, false = null = 0  
- G. 3undefined, + with a string will be a concatenation  
- H. NaN, undefined is missing value = NaN so 3 minus a NaN is NaN  

14.  
- A. true, string '2' becomes a number 2  
- B. false, both strings 2 is greater than 1  
- C. true, '2' becomes a number 2, so equal  
- D. true , checks type and value and they are the same so true  
- E. false, true = 1 so its not equal  
- F. true, Boolean(2) is true because any non zero in Boolean() is true  

15.  == checks for the value only, while === checks for both value and data type

16.  part2-question16.js

17.  returns [ 2, 4, 6], The function goes through each number in the array [1, 2, 3]. For each number, it uses the doSomething function This function multiplies the number by 2. The new values are added to a new array. So the final result is [2, 4, 6].

18.  part2-question18.js

19.  
1 <br>
4 <br>
3 <br>
2 <br>


