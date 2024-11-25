# block18-tests

## Unit Tests
**a multiplication function that renders the product of two numbers**

Expect multiplication(2,5) to return a number
Expect multiplication(2,5) to return 10
Expect multiplication(0,5) to return 0
Expect multiplication(-2, -5) to return 10
Expect multiplication(-2, 5) to return -10
Expect multiplication(2, NaN) to throw an error
Expect multiplication ("two", 5) to throw an error

** A function called "concatOdds" takes two arrays of integers as arguments and returns a single array that only contains the odd numbers, in ascending order, from both of the arrays **

Expect concatOdds([1,2,3], [4,5,6]) to return [1,3,5]
Expect concatOdds([],[4,5,6]) to return [5]
Expect concatOdds([1,2,3], [] to return [1,3]
Expect concatOdds([1,1,1,2,3], [5,5,6]) to eliminate only list one instance of duplciate numbers and return [1,3,5]
Expect concatOdds([2, 4, 6], [8, 10]) to return []
Expect concatOdds([], []) to return []
Expect concatOdds([1, "two", 3], [4, 5, "six"]) to return [1,3,5] and throw an error stating only numbers are allowed as an input
Expect concatOdds([1, 3, null], [5, undefined]) to return [1,3,5] and throw an error stating only numbers are allowed as an input
Expect concatOdds(3, [1, 2, 3]) to return [1,3] and throw an error stating input must be in the form of an array

## Functional Tests

**Shopping Cart**

*happy path*

-When the user tries to proceed to checkout with an empty cart, they should see an error message "your cart is empty" and the proceed to checkout button should be disabled

-When the user views their cart they shoudl see a list of items, quanities and prices

-When the user changes a quanity or deletes an item, that list should be updated dynamically 

-When the user proceeds to checkout, they should be met with a log in window or the option to "continue checkout as a guest"

-When the user checks out as a guest, they should be prompted to enter shipping and payment information from a blank form

-When the user logs in to check out, the same form should be presented, but with their saved data already input from the backend API

-When the user clicks "confirm purchase" they should be met with a confirmaiton page that dislayes their purchase information, and sends them an email with a receipt

*unhappy path*

-When an incorrect credit card number in input, the user should be met with a message that says "error with payment, credit card is not valid" and the purchase should not be complete

-When the user navigates away from the checkout page, their items should stay in the cart for 30 minutes

-While in the checkout process, the user should be met with a message that says "we will hold the items in your cart for 10 minutes, please checkout within that timeframe to ensure we have the items in stock"

-After 10 minutes, if an item in the users cart goes out of stock, the user should be met with a message that says "an item in your cart is now out of stock" and the quantity should change


<sup>today i learned about markdown syntax</sup>
:smiling face: