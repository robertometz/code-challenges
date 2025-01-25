### Challenge: Count the Vowels

Write a function `count_vowels/1` that takes a string and returns the number of vowels (`a, e, i, o, u`) in it. The function should be case-insensitive.

#### Example:
```elixir
count_vowels("Hello World")
# Output: 3

count_vowels("Elixir is awesome!")
# Output: 8

count_vowels("")
# Output: 0
```

#### Notes:
- Only count alphabetic vowels (ignore numbers, punctuation, etc.).
- Treat uppercase and lowercase vowels as the same.
