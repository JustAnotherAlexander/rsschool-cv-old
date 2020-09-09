# Junior Developer Resume

### About Me

My name is **Aliaksandr Matveyankou**.

### My interests

I enjoy studying computer technology and programming. I spend all my free time learning new techniques and nuances 
of programming in Javascript.
Since I love programming and technology, I decided that turning my hobby into a job is not a bad idea. This will allow 
me to apply the knowledge gained in real projects, as well as constant practice will help improve my programming skills.

### My skills:
Here is the list of my skills:
* *JavaScript*;
*  *CSS*;
* *Java*;
* *HTML*;
* *GIT*;
* *WebSocket*;

In the future, I plan to expand this list by learning new programming languages.

To apply my knowledge in practice, I'm solving tasks on the <a href="https://www.codewars.com/"> Codewars</a> website and here is my result:
<details>
<summary> My result on codeWars: </summary>
<summary> <img src="https://www.codewars.com/users/ForeverStudent/badges/large"> </summary>
</details>
I am also working on a collectible card game.

### Education

I graduated from the “Gomel Technical University named after Pavel Osipovich Sukhoi” with a degree in Hydraulics.
There I graduated from the magistracy and now i'm studing in graduate school.

### English Language

I only studied English while studying at school and university. At the moment I periodically 
read English literature and watch films in English.

### Code example

As an example, here is a small piece of code for of js function that validates the solution of Sudoku:

<details> 
<summary> here is the code of sudoku solution validator function: </summary>
  <pre>
    <code>
function validSolution(board){
var candidatesOfCell=[];
var rowIncludes = false;
var columnIncludes = false;
var squareIncludes = false;
var result =true;
 for (let row=0; row<board.length; row++) {
   for (let column=0; column<board.length; column++) {
        if (board[row][column]!=0) {
          for (let columnCounter=0; columnCounter<board.length; columnCounter++) {
            if (board[row][columnCounter]==board[row][column] && columnCounter!=column) {
             rowIncludes = true;
             }
          }
          for (let rowCounter=0; rowCounter<board.length; rowCounter++) {
            if (board[rowCounter][column]==board[row][column] && rowCounter!=row) {
              columnIncludes=true;
            }
          } 
          if (row<3) {
            for (let rowCounter2=0;rowCounter2<3;rowCounter2++) {
              if (column<3) {
                for (let columnCounter2=0; columnCounter2<3; columnCounter2++) {
                  if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
                    squareIncludes = true;
                  }
                }
              }
              if (column>=3&&column<6) {
                for (let columnCounter2=3; columnCounter2<6; columnCounter2++) {
                  if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
                    squareIncludes = true;
                  }
                }
              }
              if (column>=6) {
                for (let columnCounter2=6; columnCounter2<9; columnCounter2++) {
                  if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
                    squareIncludes = true;
                  }
                }
              }
            }
          }
          if (row>=3&&row<6) {
            for (let rowCounter2=3;rowCounter2<6;rowCounter2++) {
              if (column<3) {
                for (let columnCounter2=0; columnCounter2<3; columnCounter2++) {
                  if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
                    squareIncludes = true;
                  }
                }
              }
          if (column>=3&&column<6) {
           for (let columnCounter2=3; columnCounter2<6; columnCounter2++) {
            if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
              squareIncludes = true;
            }
          }
        }
       if (column>=6) {
        for (let columnCounter2=6; columnCounter2<9; columnCounter2++) {
          if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
            squareIncludes = true;
          }
        }
      }
    }
  }
          if (row>=6) {
    for (let rowCounter2=6;rowCounter2<9;rowCounter2++) {
      if (column<3) {
        for (let columnCounter2=0; columnCounter2<3; columnCounter2++) {
          if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
            squareIncludes = true;
          }
        }
      }
      if (column>=3&&column<6) {
        for (let columnCounter2=3; columnCounter2<6; columnCounter2++) {
          if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
            squareIncludes = true;
          }
        }
      }
      if (column>=6) {
        for (let columnCounter2=6; columnCounter2<9; columnCounter2++) {
          if (board[rowCounter2][columnCounter2] == board[row][column] && (rowCounter2!=row && columnCounter2!=column)) {
            squareIncludes = true;
          }
        }
      }
              }
            }
          if (rowIncludes!=false || columnIncludes!=false || squareIncludes!=false) {
              result = false;
            }
            }   
            rowIncludes = false;
            columnIncludes = false;
            squareIncludes = false;
        }
      }
    if (board[0][0]==0) {
        let InRow=false;
        let InColumn=false;
          for (let columnCounter=0; columnCounter<board.length; columnCounter++) {
            if (board[0][columnCounter]==board[0][0] && columnCounter!=0) {
             InRow = true;
             }
          }
          for (let rowCounter=0; rowCounter<board.length; rowCounter++) {
            if (board[rowCounter][0]==board[0][0] && rowCounter!=0) {
              InColumn=true;
            }
          }
          if (InRow!=false && InColumn!=false) {
        result = false;
    }
    }
      return result;
}
    </code>
  </pre>
</details>
