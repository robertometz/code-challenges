# Java

## Challenge
Refactor Java code using functional programming for complex calculus operations.

## Description
Given an imperative Java code performing simple math operations, refactor it using functional programming techniques like streams, lambda expressions, and method references. 

## Source code

```
public class ComplexCalculus {
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
