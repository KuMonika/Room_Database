#This project demonstrates the implementation of a Room database in an Android application using Kotlin. The application manages a list of persons, allowing users to add, edit, delete, and search for persons based on their name, age, or city.

#Features
Room Database Integration: Utilizes the Room persistence library to manage SQLite database operations in a more convenient and robust way.
Coroutines and Flow: Employs Kotlin coroutines and Flow for asynchronous programming, ensuring smooth and responsive UI interactions.
RecyclerView with DiffUtil: Efficiently updates the RecyclerView using DiffUtil, providing a smooth and performant list experience.
BottomSheetDialogFragment: Provides a modern and user-friendly interface for adding and editing person details.
Search Functionality: Allows users to search for persons by name, age, or city using a SearchView.

#Components

#Person Entity
Represents a person with attributes such as pId, name, age, and city.
Annotated with @Entity to define a table in the Room database.

#PersonDao
Defines database operations such as insert, update, delete, and search.
Uses annotations like @Insert, @Update, @Delete, and @Query to simplify SQL queries.

#AppDatabase
Abstract class extending RoomDatabase.
Provides an instance of the database and the DAO for performing operations.

#UI Components

MainActivity: Hosts the main UI components and manages the lifecycle.
AddEditPersonFragment: Bottom sheet dialog for adding or editing person details.
PersonDetailsAdapter: RecyclerView adapter for displaying the list of persons with efficient item updates.
