1. The code prints '3' to the console because it is printing the `i` variable and since the variable was defined with `var`, it's scope is throughout the function so it's last defined value is maintained when it is printed to the console.
2. The code prints '150' to the console because it is printing the `discountedPrice` variable (which is assigned to the last price in the `prices` array multplied by `(1-discount)` which is 1-0.5=0.5, so `discountedPrice` is assigned to 150) and since the variable was defined with `var`, it's scope is throughout the function so it's last defined value is maintained when it is printed to the console.
3. The code prints '150' to the console because it is printing the `finalPrice` variable (which is assigned to the last finalPrice that is pushed into the `discounted` array) and since the variable was defined with `var`, it's scope is throughout the function so it's last defined value is maintained when it is printed to the console.
4. This funciton returns the array `[ 50, 100, 150 ]`. This is because the `discounted` variable is first assigned to an empty array and then filled with the discounted values from teh `prices` array. This means that the array has `[100*0.5, 200*0.5, 300*0.5]` which is what is returned.
5. The code causes an error. This is because the code is attempting to print the `i` variable from the for loop. However, since it is defined using `let`, it is only defined within the scope fo the code block which is the for loop, therefore it cannot be accessed outside of the for loop and thus is undefined outside of the loop.
6. The code causes an error. This is because the code is attempting to print the `discountedPrice` variable from the for loop. However, since it is defined using `let`, it is only defined within the scope fo the code block which is the for loop, therefore it cannot be accessed outside of the for loop and thus is undefined outside of the loop.
7. The code prints '150' to the console. Since the `finalPrice` variable is being printed and is defined within the code block at the beginning of the funciton, it's scope is covered even if it uses `let` in its definition. Therefore, the value that is printed to the connsole is the last value that is assigned to `finalPrice` which is the rounded value of 300*0.5 which is 150.
8. The function returns the array `[ 50, 100, 150 ]`. Since the array variable `discounted` is defined at the beginning of the function with `let`, it's scope is throughout the code block which is the function itself. In the function the for loop adds the discounted prices to the array. The array that is returned is the array of the prices multiplied with `1-discount`, returning `[100*0.5, 200*0.5, 300*0.5]`.
9. The code causes an error. This is because the code is attempting to print the `i` variable from the for loop. However, since it is defined using `let`, it is only defined within the scope fo the code block which is the for loop, therefore it cannot be accessed outside of the for loop and thus is undefined outside of the loop.
10. The code prints '3' to the console. Since the `length` variable is being printed and is defined within the code block at the beginning of the function, it's scope is covered even if it uses `const` in its definition. Therefore, the value that is printed to the console is the value that it is assigned to `length` (and doesn't change) which is the length of the `prices` array (3)
11. The function returns the array `[ 50, 100, 150 ]`. Since the array variable `discounted` is defined at the beginning of the function with `const`, it's scope is throughout the code block which is the function itself. Despite being a `const`, the variable is not being reassigned to reference a different array when elements are added and therefore does not produce an error (const array references can still be changed, just not reassigned). Furthermore, `const discountedPrice` isn't reassigned through the loops, but rather have a constant definition through each iteration, therefore the respective prices are still being discounted and then added to the `discounted` array, allowing the function to return `[100*0.5, 200*0.5, 300*0.5]`.
12. Notation:
    A. `student.name`
    B. `student['Grad Year']`
    C. `student.greeting()`
    D. `student['Favorite Teacher']['name']`
    E. `student['courseLoad'][0]`
13. Arithmetic:
    A. '32': integers map to their exact string representation so the operation concatenates '3' and '2'
    B. '1': for this mathematical operation, it instead converts strings to numeric values and calculates the result as 3 - 2
    C. 3: null is converted to 0 so the operation performs 3 + 0
    D. '3null': null maps to a string so the operation concatenates '3' and 'null'
    E. 4: true converts to 1 in mathematical operations with numeric values and calculates the result as 1 + 3
    F. 0: false maps to null in numeric operations and null also maps to 0, so it calculates 0 + 0
    G. '3undefined': undefined maps toa  string so the operation concatenates '3' and 'undefined'
    H. NaN: undefined in numeric operations is converted to NaN, thus the result becomes NaN
14. Comparison:
    A. true: the string '2' is converted to the number 2 and thus returns 2 > 1.
    B. false: the two strings are compared as strings and thus in lexicographical order, meaning since the first character in '2' is '2' and the first character in '12' is '1' and since '2' comes after '1', '2' is greater than '12'.
    C. true: this is because the string is converted to its exact numeric value so 2 is seen as equivalent to 2.
    D. false: this is because three equal signs checks the equality without type conversion and thus 2 is not equal to '2'.
    E. false: true is converted to its numeric value which is 1, therefore 1 is not equal to 2
    F. true: all numeric values that are not 0, -0, or NaN will turn into true and therefore true is strictly equivalent to true
15. Both `==` and `===` will check the equivalence between the left and right side. However while `==` allows type conversion, `===` is strict equivalence and thus does not perform type conversion and accounts the type in their equivalency
16. Found in: [part2-question16.js](part2-question16.js)
17. The funciton will return the array `[ 2, 4, 6 ]`. The function `modifyArray` receives an array and callback function as parameters. Through the for loop in the function, it will go through each element in the array and call teh callback function on each element and add that to the array that is to be returned. Since the array `[1,2,3]` is passed in along with the function `doSomething` which mutliplies its input by 2, the result is that the `modifyArray` will multiply each element in `[1,2,3]` by 2 and thus return the array `[ 2, 4, 6 ]`.
18. Found in: [part2-question18.js](part2-question18.js)
19. The output is: 
    ```
    1
    4
    3
    2
    ```