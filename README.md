# Film and actor management system
This project is a Java-based application for managing films and actors. It allows users to perform various operations such as adding, editing, deleting films, managing actors, adding ratings, and saving/loading film information from a file.

## Features
- Add, edit, and delete films (both feature films and animated films).
- Add ratings to films (star ratings for feature films, point ratings for animated films).
- Manage actors and animators, including adding them to films and listing films they appear in.
- Save film details to a file and load them back into the application.
- Basic error handling and input validation.

## Usage
Once the application is running, you can interact with it via a command-line interface. Here are some key operations you can perform:
- View film details, including basic information and reviews.
- Edit film details, including name, director, and release year.
- Delete films from the database.
- Add ratings to films based on their type (star ratings for feature films, point ratings for animated films).
- Print a list of actors or animators who have appeared in more than one film.
- Print all films in the database.
- Save information about a selected film to a file.
- Load film information from a file into the application.
- Add an actor or animator to a film or remove them from a film.
- Print all actors and the movies they appeared in.

## Design principles and fundamental concepts 
### Factory method pattern
- The Factory method pattern is used in this project to create instances of films (AFilm and HFilm) based on user input. This pattern encapsulates the creation logic, allowing subclasses (AFilmFactory and HFilmFactory) to decide which type of film to instantiate without exposing the instantiation logic to the client code (Main class).
### Abstract class
- An abstract class Film is used as a base class for both feature films (HFilm) and animated films (AFilm). It defines common properties and methods such as film name, director, and release year. Subclasses implement specific details and behaviors unique to each type of film.
### Collections  
- In this project, ArrayList, TreeMap, HashSet are used to manage collections of films and actors.
### Object-oriented programming principles  
- Encapsulation, inheritance, and polymorphism are key Object-Oriented Programming principles applied throughout the project.

## Testing (JUnit)
- JUnit is used to write and run tests for the application, ensuring the correctness of various functionalities.
