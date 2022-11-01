# core-code-upskilling-readme
Core Code FullStack Bootcamp

# **Week 1:** 
## **Challenge 1**
Given a string, write a function that returns the string with a question mark ("?") appends to the end, unless the original string ends with a question mark, in which case, returns the original string.
For example (Input --> Output)

"Yes" --> "Yes?" 
"No?" --> "No?"

#### **Solution:**
<code>
    function ensureQuestion(s) {
        return (s.endsWith('?') ? s : s.concat('?'))
    }
</code>

## **Challenge 2**
Complete the solution so that it reverses all of the words within the string passed in.

Example(Input --> Output):

"The greatest victory is that which requires no battle" --> "battle no requires which that is victory greatest The"

#### **Solution:**
<code>
    function reverseWords(str){
        return str.split(' ').reverse().join(' ');
    }
</code>

## **Challenge 3**
Given an array of integers your solution should find the smallest integer.

For example:

Given [34, 15, 88, 2] your solution will return 2
Given [34, -345, -1, 100] your solution will return -345
You can assume, for the purpose of this kata, that the supplied array will not be empty.

#### **Solution:**
<code>
class SmallestIntegerFinder {
  findSmallestInt(args) {
    let smalest = Number.MAX_VALUE;
    
    args.forEach((element, index) => {
      
      if(element < args[index]) 
        smalest = element;
      else if (element < smalest)
        smalest = args[index];
      
    })
    
    return smalest;
  }
}
</code>


