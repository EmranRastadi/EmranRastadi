## binary search O(logn)

```javascript
function binarySearch(arr , target){
    let letfIndex = 0;
    let rightIndex = arr.length -1 ;

    while(letfIndex <= rightIndex){
        let middleIndex = Math.floor((rightIndex + letfIndex) / 2)
        if(target === arr[middleIndex]) return middleIndex;
        if(target < arr[middleIndex]) rightIndex = middleIndex - 1;
        else letfIndex = middleIndex + 1
    }
    return -1
}

```
