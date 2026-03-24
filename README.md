# Codewars-Count IP Addresses (Javascript)

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

[KATA](https://www.codewars.com/kata/526989a41034285187000de4/javascript)
