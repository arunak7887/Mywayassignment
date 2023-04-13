name:Arun Budhaji kinwad
email:arunkinwad02@gmail.com 
phone:7588578169
output:
1
2
3
Fizz
Buzz
6
7
Fizz
9
Buzz
11
Fizz
13
14
Buzz
Fizz
17
18
19
FizzBuzz
21
22
23
Fizz
Buzz
26
27



CODE:
function fizzBuzz() {
  const phoneNumber = prompt("Please enter your phone number:");
  
  // Calculate the sum of digits in the phone number
  const numSum = phoneNumber
    .toString()
    .split("")
    .reduce((sum, digit) => sum + parseInt(digit), 0);
  
  // Loop from 1 to the sum of digits
  for (let i = 1; i <= numSum; i++) {
    // Check if the number is divisible by 4 and 5
    if (i % 4 === 0 && i % 5 === 0) {
      console.log("FizzBuzz");
    }
    // Check if the number is divisible by 4
    else if (i % 4 === 0) {
      console.log("Fizz");
    }
    // Check if the number is divisible by 5
    else if (i % 5 === 0) {
      console.log("Buzz");
    }
    // Otherwise, just print the number
    else {
      console.log(i);
    }
  }
}

