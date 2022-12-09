1) Phone Number Selection
Set an ID for the 'tbody' where id="myTable"
<tbody id="myTable">   

```
let arr = [];
let places = document.getElementById('myTable').children;
function myFunction(place) {
    let elem = place.children
    arr.push({
        name: elem[0].textContent,
        cc: elem[1].textContent,
        iso: elem[2].textContent
    })
}

places.forEach(myFunction)
console.log(JSON.stringify(arr))
```
