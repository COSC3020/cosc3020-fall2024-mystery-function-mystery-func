# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

Answer: It takes a list or array and finds the largest value within the list and then returns it. It does this by recursively comparing the elements within the list or array until
eventually the largest element is found within the compares and returned as output. So for instance if it is given a list containing values of 7, 6, 9, 88, 21, 3 then the function will 
return 88.
