### Create Phone Number

Write a function that accepts an array of 10 integers (between 0 and 9), that returns a string of those numbers in the form of a phone number.

#### Example

```javascript
createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) // => returns "(123) 456-7890"
```

#### Solution

```javascript
function createPhoneNumber(numbers) {
  let formatNumber = "(xxx) xxx-xxxx"
  const phoneNumber = numbers.map(number => {
    formatNumber = formatNumber.replace("x", number)
  })
  return formatNumber
}
```

