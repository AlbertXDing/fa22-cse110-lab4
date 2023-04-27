#Lab 4 part 2
1. The console prints '3' because i is a var. The for loop interates through the length of prices which is 3, so i eventually equals 3. 
2. The console prints `150`. On the last iteration of the for loop, discountedPrice = 300 * 0.5 = 150.
3. The console prints `150`. On the last iteration of the for loop, discountedPrice = 300 * 0.5 = 150, thus finalPrice = Math.round(150 * 100)/100 = `150`.
4. It will return an array '[50, 100, 150]'. It can be seen that for every iteration of the loop, an element of prices is multiplied by (1-discount), rounded, and appended to discounted. So when discounted is returned, it is an array of prices * 1-discount. [100 * (1-0.5), 200 * (1-0.5), 300 * (1-0.5)] = [50, 100, 150] so that is what is returned.
5. This causes an error because i is declared with let, and thus can't be accessed outside its block which is the for loop.
6. This causes an error because discountedPrice is declared with let, and thus can't be accessed outside its block which is the for loop.
7. The console prints `150`. Unlike the issues in 5 and 6, finalPrice is declared with let but outside the for loop. Therefore the "block" it is in is the entire function. On the last iteration of the for loop, discountedPrice = 300 * 0.5 = 150, thus finalPrice = Math.round(150 * 100)/100 = 150.
8. It will return an array `[50, 100, 150]`. This is no different from question 4, because even though i and discountedPrices are declared with let inside the for loop, they are only used in the for loop. discounted and finalPrice are also declared with let, but they are outside of the loop so they can be used anywhere in the function just like a var. It can be seen that for every iteration of the loop, an element of prices is multiplied by (1-discount), rounded, and appended to discounted. So when discounted is returned, it is an array of prices * 1-discount. [100 * (1-0.5), 200 * (1-0.5), 300 * (1-0.5)] = [50, 100, 150] so that is what is returned.
9. This causes an error for because discounted can't be changed, as it is a constant. 
10. The console prints `3`. length = the length of price which is 3.
11. It will return an array `[50, 100, 150]`. In Javascript, you can still push elements to an array even if its declared as a const. The variable length is never changed, and even though discountedPrice is declared as const, it is redeclared at each iteration of the for loop, so it is reassigned a new value at each iteration. It can be seen that for every iteration of the loop, an element of prices is multiplied by (1-discount), rounded, and appended to discounted. So when discounted is returned, it is an array of prices * 1-discount. [100 * (1-0.5), 200 * (1-0.5), 300 * (1-0.5)] = [50, 100, 150] so that is what is returned.
12. 
    * A: student['name']
    * B: student['Grad Year']
    * C: student.greeting()
    * D: student['Favorite Teacher']['name']
    * E: student.courseLoad[0]
13. * A: Output: `32`. The 2 is converted into a '2'.
    * B: Output: `1`. The '3' is converted to a 3.
    * C: Output: `3`. The null acts as a 0, so 3 + 0 = 3.
    * D: Output: `3null`. '3' is a string, so null also acts as a string and is concatenated to '3'.
    * E: Output: `4`. The true is converted to 1, so 1+3=4.
    * F: Output: `0`. Both false and null are converted to 0, so it is 0.
    * G: Output: `3undefined`. undefined is converted to a string, as + can be used for concatenation, and is concatenated with '3'
    * H: Output: `NaN`. the undefined is NaN, so the operation is NaN. 
14. * A. Output: `true`. '2' is converted to 2 which is greater than 1.
    * B. Output: `false` 2 may be less than 12, but the unicode for '2' is not less than '12'
    * C. Output: `true` '2' is converted to a 2 which equals 2.
    * D. Output: `false` because of the ===, '2' is not converted to a 2, so it is not equal to 2.
    * E. Output: `false` true is converted to 1, which does not equal 2. 
    * F. Output: `true` Boolean(2) is true, so true equals true
15. === compares values without converting the types of the values it is comparing, while == does. 
16. code
17. modifyArray returns `[2,4,6]`. modifyArray essentially creates and returns an array that is the same as the array passed into it with callback being used on each element. In this case, callback is doSomething which multiplies it's argument by 2, so modifyArray multiplies each element in `[1,2,3]` by 2, thus returning `[2,4,6]`.
18. code
19. This function outputs `1`, `4`, `3`, and then 1 second later it outputs `2`. 
