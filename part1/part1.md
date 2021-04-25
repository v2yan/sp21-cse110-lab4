## Part 1a
1. values added: 20  
2. final result: 20  
3. values added: 20   
4. The code returns a reference error because ```result``` is defined within an if block with the let keyword, so it's only accessible within that scope.   
5. The code returns an error because ```result``` is a const variable, so it cannot be reassigned to ```num1 + num2```.
6. The code returns an error because there is an attempt to reassign the const ```result``` variable. 

## Part 1b
1. ```console.log(i)``` will output 3 because after the iteration of the for loop where i = 2, the i will increment to 3, and when i < prices.length is checked, the condition doesn't hold as 3 is not < 3. Thus, the for loop ends, and i retains the value of 3. Since i is function-scroped, it can be accessed anywhere in the function, so it is able to be printed outside the for loop.
2. ```console.log(discountedPrice)``` will output 150 because in the last iteration of the for loop, i = 2, so the discountedPrice = prices[2] * (1-0.5), where prices[2] = 300. Then, discountedPrice ends up with a value of 150 and is able to be printed outside the for loop because it is function-scoped. 
3. ```console.log(finalPrice)``` will output 150 because in the last iteration of the for loop, we know that discountedPrice = 150 from the previous question. When we multiply that with 100 and round it, we get 15000. Then, we divide it by 100 to get the value of finalPrice and get an end result of  ```finalPrice = 150```. Since ```finalPrice``` is function-scoped, it can be accessed anywhere in the function, so it is able to be updated within the for loop and printed outside the for loop. 
4. This function returns an array of the discounted prices: ```[50, 100, 150]```. This is because the for loop iterates through each of the prices in the array and calculates its discounted price before pushing it to a discounted array. Since there the input array had 3 prices that were to be discounted .5 (or 50%), we get all the input prices halved in the discount array. 
5. The code will return an error since i is declared with the keyword let in the for loop, which means that it is only accessible within the loop. Since ```console.log(i)``` is outside of the for loop, a reference error will occur.
6. Similar to the previous question, discountedPrice is declared with the keyword let within the for loop, which limits its accessibility to the for loop. Since ```console.log(discountedPrice)``` is outside of the for loop, a reference error will occur.
7. ```console.log(finalPrice)``` will output 150. This is because finalPrice is function-scoped as it is not declared within the for loop. This means that it is accessible within the function, which is how it's able to be updated and printed. 
8. The function returns ```[50, 100, 150]```. Like the variable finalPrice, discounted is declared outside of the for loop, making it function-scoped, and thus, accessible throughout the whole function.
9. The code will return an error because i is block-scoped, which means that it's only accessible within the for loop.
10. ```console.log(length)``` will output 3 because prices.length is unchanging, so declaring const length = prices.length won't cause an error. Since length is declared outside of the for loop, it's function-scoped, so it is accessible throughout the function. 
11. The function will return an error because discounted is a const variable that is getting updated within the for loop; const variables cannot be reassigned after its initial assignment.