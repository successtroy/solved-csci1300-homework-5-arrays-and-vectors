Download Link: https://assignmentchef.com/product/solved-csci1300-homework-5-arrays-and-vectors
<br>
<h1>Objectives</h1>

<ul>

 <li>Understand arrays and vectors.</li>

 <li>Be able to pass arrays to functions</li>

</ul>

<h1>Questions</h1>

<h2>Question 1: array pilgrimage</h2>

Write a program ​arrayPilgrimage.cpp​ to declare and populate the four arrays listed below. ● temps​ – an array of 10 floating point numbers (type ​double​) initialized with -459.67 (absolute zero in Fahrenheit)

<ul>

 <li>colors​ – an array of the strings “​Red​”, “​Blue​”, “​Green​”, “​Cyan​”, and “​Magenta​”, in that order.</li>

 <li>sequence​ – an array of the first 100 positive integers in order; ​1​, ​2​, ​3​, ​4​, … etc.</li>

 <li>letters​ – an array of all uppercase and lowercase characters in order, ​A​, ​a​, ​B​, ​b​, ​C​, ​c​, … Hint: the ASCII table will be helpful here!</li>

</ul>




In order to test that you correctly created and populated the arrays, print the values of each of their elements, in order, one element per line. ​<strong>Hint: </strong>​Use a loop to traverse each array.




Sample run

<table width="624">

 <tbody>

  <tr>

   <td width="624">-459.67-459.67 …-459.67 RedBlue…Magenta 12…100A        aB        b …Z z</td>

  </tr>

 </tbody>

</table>




The file should be named as ​arrayPilgrimage.cpp​. Don’t forget to head over to the code runner on Moodle and paste your solution in the answer box!

<strong> </strong>

<strong> </strong>Question 2: Array stats

Write a function <strong>stats</strong>​  that takes an array and the number of elements in the array. Then, it​            computes and prints the minimum value, maximum value, and the average value of all the values in the array. The output should be formatted with two-digit precision.

<em>Function specifications:  </em>

<ul>

 <li>The function name: <strong>stats</strong>​</li>

 <li>The function parameters (in this order):</li>

</ul>

○    An array, double​

○    The number of elements stored in the array, int​         ●      The function should not return anything.

Sample run 1

Test 1: 10.4 3.2 1.4 5.1 6.7

Min: 1.40

Max: 10.40

Avg: 5.36

Sample run 2

Test 2: 1 2 3

Min: 1.00

Max: 3.00

Avg: 2.00




Sample run 3

Test 3: -1.2 -12.8 5 10.4 11 2.2 -1

Min: -12.80

Max: 11.00

Avg: 1.94




The file should be named as arrayStats.cpp​        . Don’t forget to head over to the code runner​               on Moodle and paste only your function in the answer box! In the main, make sure that you call the function.

<h2>Question 3: Insert into a sorted array</h2>

Write a function <strong>insert</strong>​                that takes an array of integers in ascending order, the number of integers​ currently in the array, the total size of the array, and an integer to insert into the array. The function should insert the given integer into the array such that the array remains in sorted order. If the array is already full, the array should remain unchanged. The function should return the new number of elements in the array.

<em>Function specifications:  </em>

<ul>

 <li>The function name: <strong>insert</strong>​</li>

 <li>The function parameters (in this order):</li>

</ul>

○    An array, int​

○    The number of elements stored in the array, int​

○    The size of the array, int​

○    The new element to be added, int​

<ul>

 <li>The function returns the number of elements after inserting the element</li>

</ul>




Sample run 1

Before Insertion: 1,1,3,4,5,5,5,6

After Insertion:  1,1,2,3,4,5,5,5,6

Sample run 2

Before Insertion: 1,1,3,4,5,5,5,6

After Insertion:  0,1,1,3,4,5,5,5,6




The file should be named as insert.cpp​    . Don’t forget to head over to the code runner on​        Moodle and paste only your function in the answer box! In the main, make sure that you call the function.




<h2>Question 4:  sum of the max value found in each row</h2>

Write a function <strong>maxSum</strong>​         that takes two parameters; a 2D integer array with 10 columns, and​              the number of rows. The function must return the sum of the maximum value from each row.

<em>Function specifications:  </em>

<ul>

 <li>The function name: <strong>maxSum</strong>​</li>

 <li>The function parameters (in this order):</li>

</ul>

○   A 2D <strong>integer </strong>​ array with 10 columns​

○    The number of rows, <strong>int</strong>​ <strong>  </strong>

<ul>

 <li>The function returns the sum of the maximum value from each row as, an integer <strong> </strong></li>

</ul>




Sample run 1

Given matrix:

9  2  2  3  5  7  9  7  6  8

6  8  3  9  0  2  3  3 10  6 max sum: 19




Explanation: 9 (the highest value in the 1st row ) + 10 (the highest value in the 2nd row )  = 19.




Sample run 2

Given matrix:

5  2  8 -8  9  9  8 -5 -1 -5

4  1  8  0 10  7  6  1  8 -5

11  2 -3  8  7 10  0  3  9 11 max sum: 30




Explanation: 9 (the highest value in the 1st row ) + 10 (the highest value in the 2nd row ) + 11 (the highest value in the 3rd row )  = 30.




The file should be named as maxSum.cpp​    . Don’t forget to head over to the code runner on​        Moodle and paste only your function in the answer box! In the main, make sure that you call the function.




<h2>Question 5: Vector</h2>

Vectors are similar to arrays, but they can grow dynamically in an efficient way. Write a program that asks the user to repeatedly enter positive integers and stop when the user enters -1.

You need to use a vector in this question. At the beginning of the program, the vector is empty. Then, as the user enters values, the vector will be updated based on the following conditions in this order:

<ul>

 <li>If the vector is empty, insert the user input value into the vector</li>

 <li>If the vector is not empty and the input value is divisible by 5, then remove an element from the front of the vector</li>

 <li>If the vector is not empty and the user input value is divisible by 3, then remove an element from the end of the vector</li>

 <li>Otherwise, insert the input value at the end of the vector.</li>

</ul>




After the user is done entering values, your program should display all elements in the vector, in order, separated by spaces. On the next line, it also displays the minimum value and the maximum values in the vector.

Sample run 1 (​<strong>bold</strong>​ is user input)

<table width="624">

 <tbody>

  <tr>

   <td width="624">Please enter a number: <strong>3 </strong>Please enter a number: <strong>4 </strong>Please enter a number: <strong>7 </strong>Please enter a number: <strong>5 </strong>Please enter a number: <strong>8 </strong>Please enter a number: <strong>10 </strong>Please enter a number:<strong>-1 </strong>The elements in the vector are: 7 8Min = 7Max = 8</td>

  </tr>

 </tbody>

</table>




The file should be named as ​vector.cpp​. Don’t forget to head over to the code runner on Moodle and paste your solution in the answer box!

<h2>Question 6: split a string</h2>

When you’re processing data, it’s useful to break up a text string into pieces using a delimiter. Write a function <strong>split</strong>​    that takes a string, splits it at every occurance of a delimiter, and then​         populates an array of strings with the split pieces, up to the provided maximum number of pieces.

<em>Function specifications:  </em>

<ul>

 <li>The function name: <strong>split</strong>​</li>

 <li>The function parameters (in this order):</li>

</ul>

○    The string to be split

○    A separator, character, which marks where the string should be split up

○    An array of string, where the split-apart string pieces will be stored  ○         The size of the array, int​

<ul>

 <li>The function returns the number of pieces the string was split into, as an integer. If the string is split into more pieces than the size of the array, then it returns -1.       The function should not print anything</li>

</ul>




Sample run 1 (<strong>bold</strong>​ is user input; the array size is 4)​

<table width="624">

 <tbody>

  <tr>

   <td width="624">Enter the text: <strong>Apples,Oranges,Bananas</strong>​Enter the separator: <strong>,</strong>​ Return value: 3 arr[0] = Apples arr[1] = Oranges arr[2] = Bananas</td>

  </tr>

 </tbody>

</table>




Sample run 2 (<strong>bold</strong>​ is user input; the array size is 4)​

<table width="624">

 <tbody>

  <tr>

   <td width="624">Enter the text: <strong>2020</strong>​ <strong>//03//11 </strong>Enter the separator: <strong>/</strong>​ Return value: 3 arr[0] = 2020 arr[1] = 03 arr[2] = 11</td>

  </tr>

 </tbody>

</table>




Sample run 3 (<strong>bold</strong>​ is user input; the array size is 4)​

Enter the text:                                                 <strong>,,Tokyo,Bangalore,Boulder,London,Seattle,</strong>​

Enter the separator: <strong>,</strong>​ Return value: -1 arr[0] = Tokyo arr[1] = Bangalore arr[2] = Boulder arr[3] = London

There are 5 cities, but the size of the array is 4. Since it’s more than the size of the array, the split function returns -1.




The file should be named as split.cpp​       . Don’t forget to head over to the code runner on​        Moodle and paste only your function in the answer box! In the main, make sure that you call the function.

<h2>Extra credit: character frequency</h2>

Write a program that asks for a string. Then, it populates the counts of each character in the given string. To make it simple, the string only contains lowercase alphabetical characters from a to z. After getting the counts, print the characters and their counts in the alphabetical order, if they occur at least once in the string.




Expected output 1 (<strong>bold</strong>​ is user input)​

<table width="624">

 <tbody>

  <tr>

   <td width="624">Enter a word:<strong>colorado </strong>a: 1 c: 1 d: 1 l: 1 o: 3 r: 1</td>

  </tr>

 </tbody>

</table>




The file should be named as charCounts.cpp​        . Don’t forget to head over to the code runner​               on Moodle and paste your solution in the answer box!