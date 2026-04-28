part1: 

picture 1:
question 1: The answer printed on line 9 is 'values added: 20'.

question 2: The answer printed on line 13 is 'final result: 20'

question 3: We shouldn't use var because it can be accessed anywhere inside the function it is defined in meaning this can lead to naming conflicts and scoping issues later. Additionally, 

question 4: The answer printed on line 9 is 'values added: 20'.

question 5: This will produce an error because it is undefined when we meet the else statement. That is the let only exists inside the if statement, thus when we finish the if statement and go into the else statement everything that was inside the if statement acts like it was never there. 

question 6: This will produce an error because when you use const it means we set a variable equal to something and are never able to change it again. For example, setting result = 0 in line 5 means that result will always be equal to 0 even though we set result to be num1 + num2 on line 7.

question 7: This line will produce an error because we technically are never able to reach line 13 since line 9 also failed. However, if line 7 were be reinitialized with the result = num1 + num2 then we would be able to move onto the line 13 but it would still fail because of the same reason as in question 6, this line would be stuck on the const result = 0 on line 5.