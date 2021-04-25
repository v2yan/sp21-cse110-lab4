## Part 1a
1. values added: 20  
2. final result: 20  
3. values added: 20   
4. The code returns a reference error because ```result``` is defined within an if block with the let keyword, so it's only accessible within that scope.   
5. The code returns an error because ```result``` is a const variable, so it cannot be reassigned to ```num1 + num2```.
6. The code returns an error because there is an attempt to reassign the const ```result``` variable. 

## Part 1b
1. ```console.log(i)``` will output 3 because after the iteration of the for loop where ```i = 2```, the ```i``` will increment to 3, and when ```i < prices.length``` is checked, the condition doesn't hold as 3 is not < 3. Thus, the for loop ends, and i retains the value of 3. Since ```i``` is function-scroped, it can be accessed anywhere in the function, so it is able to be printed outside the for loop.
2. ```console.log(discountedPrice)``` will output 150 because in the last iteration of the for loop, ```i = 2```, so the ```discountedPrice = prices[2] * (1-0.5)```, where ```prices[2] = 300```. Then, ```discountedPrice``` ends up with a value of 150 and is able to be printed outside the for loop because it is function-scoped. 
3. ```console.log(finalPrice)``` will output 150 because in the last iteration of the for loop, we know that ```discountedPrice = 150```from the previous question. When we multiply that with 100 and round it, we get 15000. Then, we divide it by 100 to get the value of ```finalPrice``` and get an end result of  ```finalPrice = 150```. Since ```finalPrice``` is function-scoped, it can be accessed anywhere in the function, so it is able to be updated within the for loop and printed outside the for loop. 
4. This function returns an array of the discounted prices: ```[50, 100, 150]```. This is because the for loop iterates through each of the prices in the array and calculates its discounted price before pushing it to the ```discounted``` array. Since there the input array had 3 prices that were to be discounted .5 (or 50%), we get all the input prices halved in the ```discount``` array. 
5. The code will return an error since ```i``` is declared with the keyword let in the for loop, which means that it is only accessible within the loop. Since ```console.log(i)``` is outside of the for loop, a reference error will occur.
6. Similar to the previous question, ```discountedPrice``` is declared with the keyword let within the for loop, which limits its accessibility to the for loop. Since ```console.log(discountedPrice)``` is outside of the for loop, a reference error will occur.
7. ```console.log(finalPrice)``` will output 150. This is because ```finalPrice``` is function-scoped as it is not declared within the for loop. This means that it is accessible within the function, which is how it's able to be updated and printed. 
8. The function returns ```[50, 100, 150]```. Like the variable ```finalPrice```, discounted is declared outside of the for loop, making it scoped within the function and thus, accessible throughout the whole function.
9. The code will return an error because i is block-scoped, which means that it's only accessible within the for loop.
10. ```console.log(length)``` will output 3 because prices.length is unchanging, so  ```const length = prices.length``` won't cause an error. Since ```length``` is declared outside of the for loop, it's scoped within the function, so it is accessible throughout the function. 
11. The function will return an error because ```discounted``` is a const variable that is getting updated within the for loop; const variables cannot be reassigned after its initial assignment.
12. A) student.name   
    B) student['Grad Year']   
    C) student.greeting()   
    D) student['Favorite Teacher].name   
    E) student.courseLoad[0] (assuming first index using 0-based   indexing)   
       student.courseLoad[1] (assuming first index using 1-based
    indexing)   
13. A) '32'. 2 is converted to a string and concatenated to string '3'.   
    B) 1. '3' is converted to a number because operator - is only for numbers.   
    C) 3. Null is converted to its numeric representation 0, so 3 + 0 = 3.   
    D) '3null'. Null is converted to a string since the string '3' and the operator + are involved, which concatenates the two strings to get '3null'.   
    E) 4. True is converted to its numeric representation 1, so 1 + 3 = 4.   
    F) 0. false and null are converted to their numeric representations, both of which are 0, so 0 + 0 = 0.   
    G) '3undefined'. Undefined is converted to a string since the the other operand is a string and the operator is a +, which concantenates the two operands.   
    H) NaN. The operator - only works for numeric values, so 3 is converted to 3 while undefined is converted to NaN. Subtracting any NaN will result in NaN. 
14. A) true. '2' is converted to 2, and 2 > 1 is true. 
    B) false. Lexicographically, the first char '2' is greater than the first char '1', so '2' < '12' cannot be true. 
    C) true. '2' becomes 2, so 2 == 2 holds.
    D) false. The === operator does not do type conversion, so since 2 and '2' are different types, the statement is false.
    E) false. True is converted to its numeric value 1, and 1 is not equal to 2. 
    F) true. Boolean(2) converts 2 to its boolean value, which is true, so since both operands are booleans and are true, === returns true. 
15. The == operator does type conversions if the two operands are of different types before comparing while the === does not do type conversions before comparing, meaning if the two operands are of different types, === returns false.   
16. [16](part1b-question16.js)
17. The result is ```[2, 4, 6]```. The for loop in ```modifyArray``` iterates through each element in the input array ```[1, 2, 3]```, and passes it to the callback function ```doSomething```, which returns the element multiplied by 2. This result is then pushed onto the newArr, and the process repeats until all elements in the input array have been iterated through.
18. [18](part1b-question18.js)
19. 1    
    4   
    3   
    2  
