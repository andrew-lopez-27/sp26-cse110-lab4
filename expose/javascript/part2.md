part2: 

question 1: The answer of what line 12, console.log(i) will print out is 3, because it will continue running from i = 0 - 3 and fail on four iteration, when i = 3 because i is no longer less than prices.length it is now equal to length, that is 3 < 3.

question 2: The answer of the line 13 is 150 because it runs through iterations i = 0 - 2 while still being valid and exits at iteration i = 3, where discounted prices has increased from 50 at i = 0, 100 at i = 1, and then 150 at i = 2 after running through the for loop.

question 3: The answer of line 14 is 150, same as question 2 because when using the same explanation as question 2, when we exit the for loop for discountedPrice = 150, it is still the same logic. This time we are putting the values 50, 100, 150 through the next equations line, line 8 which is finalPrice = Math.round(discountedPrice * 100) / 100; and in this equation the 100's are cancelling out thus whatever value we in discountedPrice is the same answer as this one, thus why console.log(finalPrice) will return 150 as final answer.

question 4: The function will return an array of values, [50, 100, 150]. The way we get this is from the iterations of the for loop where the discountedPrice returns 50, 100, 150 when i = 0 - 2 and overall takes 50% off from the original value. Then it passes those values through the finalPrice which still keeps [50, 100, 150] and thus we push those values as the final discounted values. 

question 5: This code will cause an error, specifically an error saying that i is undefined because it only exists within the for loop, thus until the final iteration. Once it exits the loop and goes to line 12 it will cause delete itself and be undefined outside of the for loop, thus it ends at line 10 and is completely erased. 

question 6: This will also produce an error of discountedPrice not defined because same as question 5, discountedPrice only exists in the scope of the for loop because we are using the let keyword which means it only exist until the for loop finishes running, and thus by the time we get to line 13 the discountedPrice will no longer exist. 

question 7: This will produce the value of 150 because using the same explanation as when we were using var for getting to the answer, it will produce an array of [50, 100, 150], we don't have the let keyword on line 8 which is finalPrice and thus we aren't telling the finalPrice to only exist while the loop is alive. Thus once we finish the for loop we will still have the finalPrice which is going to be 150.

question 8: This function will produce and array of [50, 100, 150]. To get that answer we are using the same logic we used in question 4 in question 8. The reason its still the same answer is because like in question 7, we don't have the keyword let on the discounted on line 9, which means we are forever keeping the output, even after the for loop stops running. Thus, by the time we get to line 16, we will have an array of values [50, 100, 150].

question 9: This will produce an error, specifically with i being undefined because just like with let keyword in the previous questions the i in the console.log(i) will be terminated and be forgotten after the for loop because using let keyword inside the for loop means we it will be there until the loop completely terminates then be deleted from memory. 

question 10: What will happen at line 12 is that it will print the total length of the array which is 3 because it is initialized on line 4 that const length = prices.length and chceking that seeing prices is initialized at the bottom of the code on line 17, where prices is an array of size 3, thus line 12 will print a value of 3.

question 11: This function will return an array, just like in question 8, it will return an array with the values [50, 100, 150] because unlike the previous let keyword in the for loop, the discounted.push(discountedPrice) doesn't have any keywords limiting it, thus when the for loop ends, it wont delete these values from the for loops memory. Additionally, the const discountedPrice on line 7 won't affect the outcome of what is pushed to line 8.

question 12A: student.name
question 12B: student['Grad Year']
question 12C: student.greeting()
question 12D: student['Favorite Teacher'].name
question 12E: student.courseLoad[0]


question 13A: '32' 
    - The reason its '32' is because the of the '3' string in the front. When JS sees a two different types, it just assumes the second type is automatically what the first type was so in our case the int is treated as string.
question 13B: 1
    - The reason this answer is 1 is because unlike the previous part minus operand is strictly for math meaning that a string can't take a minus sign but it can take a plus thus why the last one becomes 32. But for this problem it will become 1 because it treats the string as an int because of the minus sign. 
question 13C: 3
    - The reason answer is 3, is because it treats the null as a 0 when we are performing math operations.
question 13D: '3null' 
    - Having the plus sign converts the null into a string because of the fact that the second value takes whatever type the first one is. 
question 13E: 4
    - When doing math in JS, true is automatically converted a 1. Thus 1 + 3 is 4.
question 13F: 0 
    - When doing math in JS, false and null are both converted to 0. Thus 0 + 0 = 0.
question 13G: '3undefined'
    - Same reasoning as 13D, when doing addition with strings as the first type whatever is on the right side of the plus sign is automatically converted into a string type.
question 13H: NaN
    - The way we get NaN is because having the minus sign, automatically makes this be a math operation and thus having undefined with a math operations sets undefined = NaN. Thus 3 - NaN = NaN


question 14A: true
    - The reason this evaluates to true is because when comparing a string with an int, JS converts the string to a number thus '2' turns into 2 which is greater than 1, thus true.
question 14B: false
    - Since both are strings rather than converting to the strings to ints, it compares their lexicographical characters. It compares '2' and '1' and since it sees that '2' > '1' then it automatically thinks that '2' is also greater than '12'.
question 14C: true
    - Same reasoning as 14A, having == converts the string to int since we have at least one int value already and thus 2 is equal to 2.
question 14D: false 
    - Using the === checks for strict equality of both values and types, thus why it fails because it is comparing ints and strings. 
question 14E: false 
    - When comparing a boolean with ints, it converts the boolean to an int and thus true is converted to a 1 and thus the statement becomes false because 1 != 2.
question 14F: true
    - What it does is it converts the Boolean(2) to 2, but also in JS since we don't have another int Boolean(2) is also converted to true. Thus true === true.


question 15: The difference between == and === is that "==" checks for loose equality meaning it automatically converts the values to the same data types such as string and int converts the string to an int, then compares. But for the "===" it strictly checks for both value and type and checks if they match. So if one of those are false then the statement automatically becomes false. 

question 16: on part2-question16.js file

question 17: The result of modifyArray([1, 2, 3]) will be [2, 4, 6]. This is the process of how we got this answer. First, since we see that modifyArray([1,2,3], doSomething) is defined at the bottom of the code on line 13 and we see the length of the array is 3 this the for loop we set array.length = 3, so the loop runs until i = 3. From here we go into the modifyArray function and set the empty newArr equal to the values of the modifyArray, thus [1,2,3]. For the first iteration of the loop, we start at i = 0 and check if its smaller than array.length which it is so we move onto the next line, newArr.push(callback(array[i])), and we set the value at i = 0 equal to 1. We then do that until the for loop no passes, that is when i = 3. This gives us an array of [1,2,3]. These values are then pushed into the doSomething function where each is individually multiplied by 2, thus 1 * 2 = 2, 2 * 2 = 4, 3 * 2 = 6, and the newArr = [2, 4, 6].

question 18: on part2-question18.js file

question 19: The output of the code goes as follows 
    - 1
    - 4
    - 3
    - 2
      - The way we get these values is by in JS timers are looked at as second in line so we execute all the lines that can be executed instantly, such as lines 2 and 5. Thus why we start with order 1, 4. From here deciding between 2 and 3 is solely based on the delay of the two. Since console.log(2) has a 1000 ms delay and console.log(3) has 0 ms delay 3 comes before 2. Thus our final order is 1, 4, 3, 2.
