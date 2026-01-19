# My-Movies-app

A web application built with ASP.NET Core MVC that allows users to manage a collection of movies.

## Overview

My-Movies-app is a Movie Management System developed as part of a CSE325 course project. It provides a user-friendly interface for adding, viewing, editing, and deleting movie records from a database.

## Features

- **Movie Database**: Store and manage movie information including title, release date, price, genre, and rating
- **CRUD Operations**: Create, read, update, and delete movie records
- **Search & Filter**: Browse through movies in your collection
- **Data Validation**: Input validation for movie attributes
- **Responsive Design**: Bootstrap-based UI for a clean, modern user experience

## Technology Stack

- **Framework**: ASP.NET Core MVC (.NET 10.0)
- **Database**: SQLite with Entity Framework Core
- **Frontend**: Razor Views, Bootstrap, jQuery
- **Language**: C#

## Movie Model

Each movie in the database contains:

- **Title**: Movie name (3-60 characters)
- **Release Date**: Date when the movie was released
- **Price**: Movie price (decimal value)
- **Genre**: Movie genre (required, starts with capital letter)
- **Rating**: Movie rating (up to 5 characters, e.g., PG, PG-13, R)

## Project Structure

- `Controllers/`: Contains MVC controllers (HomeController, MoviesController, HelloWorldController)
- `Models/`: Movie model and view models
- `Views/`: Razor templates for rendering pages
- `Data/`: Database context configuration
- `Migrations/`: EF Core migrations for database schema
- `wwwroot/`: Static assets (CSS, JavaScript, Bootstrap libraries)

## Getting Started

1. Clone the repository
2. Navigate to the MvcMovie directory
3. Restore dependencies: `dotnet restore`
4. Create and seed the database: `dotnet ef database update`
5. Run the application: `dotnet run`
6. Open your browser and navigate to `https://localhost` to access the app

## Database

The application uses SQLite for data persistence with Entity Framework Core for data access. Database migrations are included to set up the initial schema and apply updates.
