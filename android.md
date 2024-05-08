# Android

## Challenge
Create a simple Android app with Kotlin that fetches data from a public API and displays it in a list.

## Requirements
1. Use the JSONPlaceholder API: https://jsonplaceholder.typicode.com/
2. Fetch data from the API using Retrofit or any other HTTP client library
3. Perform network operations asynchronously to avoid blocking the main UI thread and maintain a smooth user experience
4. Display the fetched data in a RecyclerView
5. Each item in the list should display at least two pieces of information from the API response (e.g., title and body for posts)
6. (Optional) When an item in the list is clicked, display a detail view with more information about the selected item

## Technical Questions
- Explain the role of the RecyclerView in Android UI development and how it improves performance compared to the older ListView.
- What are the benefits of using Kotlin Coroutines over traditional threading approaches (e.g., AsyncTask, Thread)? Can you provide examples of how you would use coroutines in an Android app?
