# Java

## Challenge
Refactor Java code using functional programming.

### Description
Given an imperative Java code performing simple math operations, refactor it using functional programming techniques like streams, lambda expressions, and method references. 

### Source code

```
public class SumAndAverage {
    public static void main(String[] args) {
        int[][] matrix = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
        int sum = 0;
        for (int[] row : matrix) {
            for (int num : row) {
                sum += num;
            }
        }
        double average = (double) sum / (matrix.length * matrix[0].length);
        System.out.println("Sum: " + sum);
        System.out.println("Average: " + average);
    }
}
```

## Technical Questions
1. Explain the concept of method overloading and method overriding in Java. Provide an example of each.
2. What is a functional interface in Java, and why is it important?
3. What do @Component, @Service, @Repository, and @Controller annotations represent in Spring Boot?
4. How does Spring Boot handle dependency injection, and what are its methods?
5. What are Spring Boot starters, and can you name some common examples?
