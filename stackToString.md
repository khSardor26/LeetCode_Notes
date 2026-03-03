# 📌 Java Stream Example – Converting Stack to String

stack.stream()  
  .map(Object::toString)  
  .collect(Collectors.joining(""));

## 🔎 What This Code Does

This code converts all elements of a `Stack` into a single concatenated `String`.

----------

## 🧩 Step-by-Step Breakdown

### 1️⃣ `stack.stream()`

Creates a **Stream** from the `stack` collection.

-   Allows functional-style operations
    
-   Processes elements sequentially (by default)
    

----------

### 2️⃣ `.map(Object::toString)`

Converts each element in the stack to a `String`.

-   `Object::toString` is a **method reference**
    
-   Equivalent to:
    

.map(element -> element.toString())

This ensures that even if the stack contains integers, characters, or custom objects, they are converted into text form.

----------

### 3️⃣ `.collect(Collectors.joining(""))`

Collects all mapped strings and joins them together.

-   `Collectors.joining("")` merges strings
    
-   Empty string `""` means **no separator**
    

Example:

If stack contains:

['a', 'b', 'c']

Result:

"abc"

----------

## 📌 Practical Example

Stack<Character> stack  =  new  Stack<>();  
stack.push('H');  
stack.push('e');  
stack.push('y');  
  
String  result  =  stack.stream()  
  .map(Object::toString)  
  .collect(Collectors.joining(""));  
  
System.out.println(result);

Output:

Hey

----------

## 🎯 Why Use This?

✔ Clean and readable  
✔ Functional programming style  
✔ Avoids manual loops  
✔ Works with any object type
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg1NTc3MTI0OV19
-->