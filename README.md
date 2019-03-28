# FriendFinder

## Description
This is an application for finding friends based on ten short survey questions with answers ranging from 1 [strongly disagree] to 5 [strongly agree]. This full-stack site will take in results from users' surveys, then compare their answers with those from other candidates and users in the database. The app will then display the name and picture of the user with the best overall match.

To determine the user's most compatible friend we used the following logic:
* Convert each user's answers into a simple array of numbers (ex: `[5, 1, 4, 4, 5, 1, 2, 5, 4, 1]`).
* With that done, compare the difference between current user's scores against those from other users, question by question. Add up the differences to calculate the `totalDifference`.
* Example:
  * User 1: `[5, 1, 4, 4, 5, 1, 2, 5, 4, 1]`
  * User 2: `[3, 2, 6, 4, 5, 1, 2, 5, 4, 1]`
  * Total Difference: **2 + 1 + 2 =** **_5_**
* Use the absolute value of the differences & No negative solutions! 
* The closest match will be the user with the least amount of difference.

## Preview
Please preview the app [here](https://sheltered-spire-56824.herokuapp.com/)

## Built With Following Technology
* HTML
* JavaScript
* jQuery
* Node.js
* NPM Package
  * Body-Parser 
  * Express 
  * Path 
  
## Author
* *Sonam* 





