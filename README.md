# GenomicRangeQuery
## Javascript - Codility Genomic Range Query 100%
## time complexity: O(N + M)

```
let S = "CAGCCTA";
let Q = [4,5,6];
let P = [2,5,0];


function solution(S, P, Q) {
    // write your code in JavaScript (Node.js 8.9.4)
    
 let result = [];

for (i=0;i<=S.length; i++){
  let SL = S.slice(P[i],Q[i]+1);

  if(SL.indexOf("A") !== -1){
    result.push(1);
  }else if(SL.indexOf("C") !== -1){
    result.push(2);
  }else if (SL.indexOf("G") !== -1){
    result.push(3)
  }else if(SL.indexOf("T") !== -1){
    result.push(4)
  }
}

return result;
```
