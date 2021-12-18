1. Construct a function intersection that compares input arrays and returns a new array with elements found in all of the inputs. You can only use reduce method to do this.

```js
function intersection(...arrays) {
  return arrays.reduce((acc,cv,index,arr)=> {
 if(index>0){
     if(index>1){     
        let temp=[];
          for (let i=0;i<acc.length;i++)
            {

              for (let j=0;j<cv.length;j++)
              {
                 if(acc[i]==cv[j])
                 {
                  temp.push(acc[i]);
                 }
              }
            }
      acc=temp
    }
    
    else{

         for (let i=0;i<arrays[0].length;i++){
            for (let j=0;j<cv.length;j++){
              if(arr[0][i]===cv[j]){
               acc.push(arrays[0][i])
              }
           }
         }
     } 

  
  }
  
 
  return acc;
  },[])
}



// Test
console.log(
  intersection(
    [5, 10, 15, 20],
    [15, 88, 1, 5, 7],
    [1, 10, 15, 5, 20]
  )
); // should log: [5, 15]
```

2. Construct a function `union` that compares input arrays and returns a new array that contains all elements. If there are duplicate elements, only add it once to the new array. Preserve the order of the elements starting from the first element of the first input array. You can only use reduce method to do this.

```js
function union(...arrays) {
   return arrays.reduce((acc,cv,index,arr)=> {
     if(index>0){
          for (let i=0;i<cv.length;i++)
            {

              for (let j=0;j<acc.length;j++)
              {
                 if(cv[i]!==aac[j])
                 {
                  acc.push(cv[i]);
                 }
              }

            }
          }else{
            acc = cv;
          }
   
  
  
 
  return acc;
  },[])

}

// Test
console.log(
  union([5, 10, 15], [15, 88, 1, 5, 7], [100, 15, 10, 1, 5])
);
// should log: [5, 10, 15, 88, 1, 7, 100]
```
