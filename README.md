# Mystery Function
“I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”
No sources were used to complete this exercise.

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
The mystery function recursively removes the leading character of any string passed in until only the last character in the string remains and then returns that character. If the array contains numbers, it still recursively removes the value at index 0 until the array size is 1, except in the case that the value in index 0 is larger than any other individual value in the index, in which case it returns the value currently in index 0.
