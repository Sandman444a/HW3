## a

The Average function takes the first k elements in an array and returns the average. If the number of k elements is greater than the number of total elements in the list, it will just take the entire list and find the average.

## b

For our basic test cases, we will simply try to make a list with few elements, consisting of numbers that we can easily average in our minds. We will then take the first k elements of said list and see if our average matches what it should be.

## c

###The following will be our partition test cases (every possible scenario we should account for).

Obtaining the average of the first k elements in the list.
Obtaining the average of the entire list (when k is greater than the list size).
Obtaining the average of an empty list.
Obtaining the average when k = 0.
Obtaining the average with negative numbers.
Obtaining the average if k is negative.
Obtaining the average of 1 element in the list.

## d

Our boundary value test cases seem to have been solved as we did our partition test cases. Values for k that we'd be concerned about are 0, any negative number, or 1 above the number of list elements, which have been dealt with and have had no faults.

## e

![image_2024-12-07_121656487](https://github.com/user-attachments/assets/16e0de32-7034-4d12-af91-abad69c6c445)


## f

For my testing, I had issues getting my Asserttrue method to run properly. Luckily Eclipse was helpful in telling me that I was trying to call a integer array non statically, which made me realize that the original average method in the Average class was not static. After fixing this, it would run properly.
When I did all of my test cases, the only one to fail was K greater than, but that was due to human error (I had the average set as 3, when it should have been 4).

##g

In the coverage testing, I achieved a 95.8% on branch coverage for AverageTest.java, missing 1 (unclear) instruction in every test case. Considering these branches are mutually exclusive, it's otherwise difficult to get an exact 100% coverage

![image_2024-12-07_124740819](https://github.com/user-attachments/assets/8526b142-1fd8-4e75-b352-46eb34f19a5b)

