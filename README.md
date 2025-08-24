# JavaScript Algorithms and Data Structures Course by FreeCodeCamp

## STEP 1
 
 A teacher has finished grading their students' tests and needs your help to calculate the average score for the class.

 Complete the getAverage function which takes in an array of test scores and returns the average score.

 The average is calculated by adding up all the scores and dividing by the total number of scores.

## Example Code
**average** = **sum of all scores** / **total number of scores**
A couple of function calls have been provided for you so you can test out your code.

## Tips

- You can use a loop to iterate over the scores array and add up all the scores.
- You can use the length property to get the total number of scores.





```javascript
function getAverage(scores) {
    let sum = 0;
    for (let i = 0; i < scores.length; i++) {
    sum += scores[i];
    
  }
  let total = scores.length;
  let average = sum/total;
  return average
 
}

console.log(getAverage([92, 88, 12, 77, 57, 100, 67, 38, 97, 89]));
console.log(getAverage([45, 87, 98, 100, 86, 94, 67, 88, 94, 95]));
```

## Step 2

 Now the teacher needs your help converting the student score to a letter grade.

 Complete the getGrade function that takes a number score as a parameter. Your function should return a string representing a letter grade based on the score.

 Here are the scores and their corresponding letter grades:

 # Example Table

| Score Range | Grade |
|-------------|-------|
| 100         | A++   |
| 90-99       | A     |
| 80-89       | B     |
| 70-79       | C     |
| 60-69       | D     |
| 0-59        | F     |


```javascript
function getGrade(score) {
  if (score === 100)  {
    return "A++"
  } else if ( score >= 90) {
    return "A"
  } else if ( score >= 80) {
    return "B"
  } else if ( score >= 70) {
    return "C"
  } else if ( score >= 60) {
    return "D"
  } else if ( score <= 59) {
    return "F"
  }
}

console.log(getGrade(96));
console.log(getGrade(82));
console.log(getGrade(56));
console.log(getGrade(20));
```
