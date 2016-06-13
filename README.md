# Bootcamp Prep: Recursion

Recursion: Calling a function on itself

Coderbyte Challenge: First Factorial
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

Termination condition: base case is a form of termination condition. However what if user input is not covered by base case? Must use additional condition as back up.

    function factorial(n) {
    if(n < 0) {
    // termination condition to prevent infinite recursion
       return;
    }
    if(n===0){
    // base case
       return 1;
    }
    // recursive case
       return n * factorial(n-1);
    }
    factorial(-1);
    factorial(5);
    
