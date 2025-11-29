# CineScope

<p align="center">
  <a href="https://youtu.be/BaBvsk_b4Cs" target="_blank">
  </a>
</p>

CineScope is a Spring Boot MVC web application for managing a movie catalog, enabling users to add, view, update, delete, and search movies stored in a MySQL database.

## Project Overview

CineScope delivers an end-to-end flow for maintaining movie records, from database persistence to user-facing views. The application follows a Controller–Service–Repository pattern with JPA/Hibernate handling data access and Thymeleaf rendering dynamic HTML templates.

## Core Features

- Full CRUD operations for movie entities (create, read, update, delete).
- Search functionality to look up movies by name from a relational database.
- Clear layered architecture (Controller → Service → Repository) for separation of concerns.
- JPA/Hibernate integration with MySQL for persistence and querying.
- Preloaded sample data to simplify testing and demonstrations.
- User-friendly Thymeleaf pages for listing, editing, and managing movie details.

## Technology Stack

- **Backend:** Java, Spring Boot, Spring MVC  
- **View Layer:** Thymeleaf  
- **Persistence:** Spring Data JPA / Hibernate, MySQL  
- **Build & Dependencies:** Maven  

## Installation and Setup

1. **Clone the repository**

  git clone https://github.com/HARSHEE04/CineScope.git

  cd CineScope

2. **Create the MySQL database**
   
   
 CREATE DATABASE cinescope;

 3. **Configure application properties**
    
Update `src/main/resources/application.properties` with your own credentials:

spring.datasource.url=jdbc:mysql://localhost:3306/cinescope
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update

**Open CineScope in your browser**

http://localhost:8080/main

## Usage Guide

- Navigate to the main movies page to view all existing entries.
- Use the “Add” flow to create new movies (e.g., title, genre, release year, description).
- Edit or delete movies directly from the list to maintain the catalog.
- Use the search bar to quickly find movies by name.
