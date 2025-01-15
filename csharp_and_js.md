# Code Challenge

### C#: Find the Longest Word in a Sentence

**Challenge Description:**

Write a C# program that takes a sentence as input and determines the longest word in it. If there are multiple words with the same maximum length, return the last one.

---

**Requirements:**

1. Implement a method `FindLongestWord(string sentence)` that:
   - Returns the longest word in the sentence.
   - Ignores punctuation and treats words as sequences of alphabetic characters.
2. Handle empty strings gracefully by returning an empty string.
3. Consider words separated by spaces only.

---

**Input Examples:**

- Input: `"The quick brown fox jumps over the lazy dog."`  
  Output: `"jumps"`  

- Input: `"I love programming in CSharp!"`  
  Output: `"programming"`

- Input: `""`  
  Output: `""`

---

**Starter Code:**

```csharp
using System;

public class Program
{
    public static string FindLongestWord(string sentence)
    {
        // Your implementation here
    }

    public static void Main(string[] args)
    {
        Console.WriteLine(FindLongestWord("The quick brown fox jumps over the lazy dog.")); // Expected output: "jumps"
        Console.WriteLine(FindLongestWord("I love programming in CSharp!")); // Expected output: "programming"
        Console.WriteLine(FindLongestWord("")); // Expected output: ""
    }
}
```

---

**Expected Output:**

```plaintext
jumps
programming

```

### JS: Rank Cities by Population

**Challenge Description:**

Write a JavaScript function that processes a list of cities and their populations. The function should:

1. Filter out cities with a population of 2 million or less.
2. Rank the remaining cities by their population in descending order.
3. Return a new list where each city object includes an additional field, `rank`, indicating its position in the ranking.

---

**Input Example:**

```javascript
let cities = [
    { name: 'Los Angeles', population: 3792621 },
    { name: 'New York', population: 8175133 },
    { name: 'Chicago', population: 2695598 },
    { name: 'Houston', population: 2099451 },
    { name: 'Philadelphia', population: 1526006 }
];
```

---

**Expected Output:**

```javascript
[
    { name: 'New York', population: 8175133, rank: 1 },
    { name: 'Los Angeles', population: 3792621, rank: 2 },
    { name: 'Chicago', population: 2695598, rank: 3 },
    { name: 'Houston', population: 2099451, rank: 4 }
]
```
