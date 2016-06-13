# Codebyte-Challenge-First-Factorial
Have the function FirstFactorial(num) take the num parameter being passed and return the factorial of it (ie. if num = 4, return (4 * 3 * 2 * 1)). For the test cases, the range will be between 1 and 18. 


    function FirstFactorial(num) {
    // Base case, when num is equal to 0, stop recursion
    // if you dont have base case, then recursion will go on forever and program will crash.
      if(num === 0) {
      return 1;
      }
    // this is recursive case
    // it will run for all other conditions except when num is equal to 0
    return num * FirstFactorial(num - 1);
    }
