# week1_day5
OOP

----

## Solución LAB 13-jul

````javascript
// Iteration #1: Find the maximum
const maxOfTwoNumbers = (val1, val2) => val1 > val2 ? val1 : val2




// Iteration #2: Find longest word
const words = ['mystery', 'brother', 'aviator', 'crocodile', 'pearl', 'orchard', 'crackpot'];

function findLongestWord(wordsArray) {
  if (wordsArray.length === 0) {
    return null
  }
  if (wordsArray.length === 1) {
    return wordsArray[0]
  }

  let longestWord = ''

  wordsArray.forEach(function (eachWord) {
    if (eachWord.length > longestWord.length) {
      longestWord = eachWord
    }
  })

  return longestWord
}



// Iteration #3: Calculate the sum
function sumNumbers(numbers) {

  if (!numbers.length) {
    return 0
  }

  if (numbers.length === 1) {
    return numbers[0]
  }

  let sum = 0

  numbers.forEach(function (eachNumber) {
    sum += eachNumber
  })

  return sum
}




// Iteration #4: Calculate the average
// Level 1: Array of numbers
const numbersAvg = [2, 6, 9, 10, 7, 4, 1, 9];

function averageNumbers(numbers) {

  if (numbers.length === 0) {
    return null
  }

  const sum = sumNumbers(numbers)

  return sum / numbers.length
}


// Level 2: Array of strings
const wordsArr = ['seat', 'correspond', 'linen', 'motif', 'hole', 'smell', 'smart', 'chaos', 'fuel', 'palace'];

function averageWordLength(words) {

  let sumLengths = 0

  words.forEach(function (eachWord) {
    console.log('ESTA PALABRA ES', eachWord)
    console.log('ANTES EL SUMATORIO ERA DE', sumLengths)
    sumLengths += eachWord.length
    console.log('AHORA EL SUMATORIO ERA DE', sumLengths)
    console.log('------')
  })

  return sumLengths / words.length
}


// Iteration #5: Unique arrays
function uniquifyArray(arr) {

  let newArr = []

  arr.forEach(function (eachWord) {

    console.log('LA PALABRA ES', eachWord)

    if (newArr.includes(eachWord)) {
      console.log('¡¡¡¡OJO!!!!', eachWord, 'NO ESTA EN EL ANTERIOR ARRAY')
      newArr.push(eachWord)
    }

    console.log('-----')
  })

  return newArr
}
````
