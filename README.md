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
The mystery() function takes an array a. It sets a base case of the length of the array being 1, to return the first indexed element. 
The variable foo is used to take the mystery function output when it slices the array to make a new one, where it slices the first element and begins a new array with the next element up till the end of the array. This continues recursively until the length is one. Once it has reached the length of one or foo, foo will compare itself to the previous first indexed elements to see if its greater than them. If it is not greater, it will be replaced by the other element or stay as foo that will eventually return the highest value in the array once it has gone through all of the elements.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
