# MyApiApp
 
My Assssment Application
Overview
My Assssment Application is an Android app that lets users log in and see a list of items from an online service. It has three screens:
·       Login: Users enter their name and ID to sign in.
·       Dashboard: Shows a list of items related to the user.
·       Details: Shows more information about a selected item.
The app talks to the online API at https://nit3213api.onrender.com/.
Features
·       User login with username and password.
·       Shows a list of items from the API.
·       Can handle items with different kinds of information.
·       Uses a clean way to organize code with dependency injection.
·       Lists items with RecyclerView.
·       Shows detailed info for each item.
·       Logout button to return to login.
Project Structure
·       ApiService: Interface for API calls.
·       MainActivity: Login screen.
·       DashboardActivity: Shows list of items.
·       DetailsActivity: Shows details of one item.
·       Entity: Data model for items.
·       EntityAdapter: Adapter for showing list of items.
·       EntityDeserializer: Helps parse dynamic item data.
·       NetworkModule: Provides Retrofit and Gson objects.
·       Layout files: XML files for the UI.
Setup Instructions
Requirements
·       Android Studio
·       Android device or emulator with SDK 28+
·       Internet connection
Steps
1.   Open the project in Android Studio.
2.   Build the project (Gradle will download required libraries).
3.   Run the app on your device or emulator.
Usage
1.   Open the app.
2.   Enter your first name and student ID.
3.   Tap Login.
4.   After login, see the list of items on the dashboard.
5.   Tap any item to see details.
6.   Use Back button to return to dashboard.
7.   Tap Logout to go back to login.
Notes
·       The app uses a special parser to handle items with different properties.
·       Shows error messages if network calls fail.
·       Uses Kotlin, Retrofit, Gson, and Dagger Hilt libraries.
·       Backend API URL: https://nit3213api.onrender.com/
·       The UI is simple and easy to use.
Dependencies
·       Retrofit for API calls
·       Gson for JSON parsing
·       Dagger Hilt for dependency injection
·       AndroidX libraries for UI components
File Summary
·       MainActivity.kt: Login logic
·       DashboardActivity.kt: List items and fetch data
·       DetailsActivity.kt: Show item details
·       Entity.kt: Data model
·       EntityAdapter.kt: Adapter for RecyclerView
·       EntityDeserializer.kt: Parse dynamic JSON
·       NetworkModule.kt: Setup Retrofit and Gson
·       XML layout files: UI design
License
This project is for learning purposes only.
 
