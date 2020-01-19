# Is-a-number-prime

function isPrime(num) {
    let i = 2;
    if (num < 2) {
        return false;
    } else {
        while (i <= num/2) {
            if (num % i === 0) {
                return false;
            } else {
                i++;
            }
        }
    }
    return true;
}
  isPrime()
  console.log(isPrime());


  // faster 
  function isPrime(num) {
    for(let i = 2, a = Math.sqrt(num); i <= a; i++)
            if(num % i === 0) return false; 
        return num > 1;
    }
    console.log(isPrime(6));
