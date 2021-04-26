## Part 1A
1. values added: 20
2. final result: 20
3. values added: 20
4. Returns an error because result is not declared within the scope of the console.log on line 13. result is only defined inside of the if statement.
5. Code returns an error because you are trying to reassign the value of a const variable
6. Code returns an error because result is not within the scope of line 13's console.log. result is only defined inside of the if statement.

## Part 1B
1. The code will print 4 into the console because i is declared as a var. Since it is a var, the variable i is not restricted to the for loop. Rather, it can be used outside the scope it was declared in. In other words, variable i is a global variable and as such you can use it anywhere after declaring/initializing it.
2. Line 13 will print out 150 because discountedPrice's last reassignment was when i was equal to 2. The value of prices[2] was 300 and multiplying that number by (1 - .5) gives us 150. Since the variable is declared as a var type, it can be used outside of the for loop.
3. finalPrice is a var. What this means is that at line 14 the value of finalPrice will be outputted because finalPrice is globally scoped. That value is 150. This is because on line 8 finalPrice's last reassignment is Math.round(150 * 100) / 100 = 150.
4. The function will return [50, 100, 150] because discounted is an array where we pushed those 3 elements into. The function just applies the given discount onto the elements found in the prices array. It also rounds it to 2 decimal places.
5. This code will cause an error at line 12 because the variable i is not defined outside of the for loop. The let declaration restricts the variable's scope to the block it was initialized in.
6. Line 13 will cause and error because discountedPrice is not defined within the scope of the discountPrices block. Instead, discountedPrice is restricted to the for loop starting at line 6 and ending at line 10.
7. Line 14 will output 150 because finalPrice was declared within the main discountPrices scope and the last reassignment in the for loop set finalPrice was 150.
8. The function will return [50, 100, 150] because discounted price is an array that contains those 3 values. The function takes in all the prices that are going to be discounted and creates the array, discounted. It pushes the discounted price into the discounted array and returns the discounted array.
9. Line 11 would throw an error because i is not defined outside the scope of the for loop.
10. Line 12 will output 3 because the length of the prices array is 3. The length array's scope is that of the discountPrices function.
11. The function will return [50, 100, 150] once again. The reason is because there is a new discountedPrice variable being declared and initialized on line 7. This doesn't cause an error because we are not trying to reassign the const variable. Rather, we are creating a new const variable every iteration of the for loop because after the last itr finishes the previou discountedPrice variable is forgotten and that allows us to create discountedPrice. As for another overview of the function, we have a const variable assigned to an array which just means that the variable cannot point to any other arrays. However, it can still manipulate the object by adding or subtracting elements because that is not reassigning the value of the original variable.
12. Write the notation
    1.  student['name']
    2.  student['Grad Year']
    3.  student.greeting()
    4.  student['Favorite Teacher']['name']
    5.  student['courseLoad'][0]
13. Arithmetic
    1.  '3' + 2 = '32' - The + operator can also be used for concatentation. Since the first input is a string and the second one is an int, the int converts to a string and the two are concatenated.
    2.  '3' - 2 = 1 - The - operator does not work with string values. As such, it converts the '3' into an int and subtracts the int 3 by the int 2.
    3.  3 + null = 3 - null gets converted to a 0 and 3 + 0 = 3.
    4.  '3' + null = '3null' - This occurs because '3' is a string and it thus converts null into a string as well and concatenates the two.
    5.  true + 3 = 4 - true is the same thing as 1. So converting true to the int value 1 gives us 1 + 3 = 4
    6.  false + null = 0 - false and null when converted to an int is 0. So we have, 0 + 0 = 0
    7.  '3' + undefined = '3undefined' - undefined gets converted into a string and is concatenated with 3 to give us '3undefined'
    8.  '3' - undefined = NaN - While the - operator tries to convert '3' and undefined into integers, we find that undefined's numerical value is NaN (not a number). Trying to do arithmetic with something that is NaN will give us NaN.
14. Comparison
    1.  '2' > 1 == true because '2' gets converted into a numeric value and 2 > 1 is true.
    2.  '2' < '12' = false because if both inputs are strings, then the < operator compares 1 character at a time. Since '2' > '1', the result of '2' < '12' is false.
    3.  2 == '2' = true because '2' gets converted into a numeric 2 and 2 == 2.
    4.  2 === '2' = false because 2 and '2' are different data types and the === operator checks for types as well.
    5.  true == 2 = false because true will be converted to the numeric value of 1 and 1 != 2.
    6.  true === Boolean(2) = true because Boolean(2) creates a boolean with the value of true. Since both sides are booleans and both sides are also true, then the comparison is true. Boolean(2) creates a boolean with the value true because the only way to create a Boolean with the value false using Boolean() is by setting the input as 0, -0, null, false, NaN, undefined, or the empty string ("").
15. The difference between == and === is that === checks that the two values are the same data type as well while == does not. == will attempt to convert one or both values into the same one before comparing. So in other words, === does not convert values.
16. Check part1b-question16.js file
17. The function will return [2,4,6]. Stepping through the function, we can note that the parameters include: an array of numeric values and a function. We first set up the newArr array that we are going to be storing the new values into. Next we have a for loop that goes through all the elements in the array parameter and pushes the result of running the callback function on each value in array. The callback variable is actually just the doSomething function. The doSomethingfunction multiples the given input by 2 and returns that value. That is the value that is being stored into newArr. Once all the numbers are multiplied by 2, we return newArr.
18. Check part1b-question18.js
19. It will print 1 4 3 2 on separate lines in that order. The reason why line 5 executes before line 4 despite line 4 having a delay of 0 is that the delay is not exactly accurate. So even though it says 0, it is slightly longer than that which is still longer than it actually being 0.