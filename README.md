# Codewars-Count IP Addresses (Javascript)
1. 
```
function ipsBetween(start, end){
  start = start.split('.').reduce((accumulator, currentValue, currentIndex) => {
    return accumulator += currentValue * Math.pow(256, 3 - currentIndex);
  }, 0);
  
  end = end.split('.').reduce((accumulator, currentValue, currentIndex) => {
    return accumulator += currentValue * Math.pow(256,  3 - currentIndex);
  }, 0);
  
  return end - start;
}
```
2. 
```
function ipsBetween(start, end){
  start = start.split('.');
  const result = end.split('.').map((v, i) => v - start[i]);
  
  return result.reduce((acc, v, i) => acc += v * Math.pow(256, 3 - i), 0);
}
```
---

[KATA](https://www.codewars.com/kata/526989a41034285187000de4/javascript)
