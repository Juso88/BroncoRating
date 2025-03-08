# BroncoRating

## Project Description
BroncoRating is a web platform where students can rate professors and other students, fostering constructive feedback in academic settings.

## Key Features
- **User Authentication** – Secure login system with role-based access for students, professors, and admins.  
- **Rating System** – Students can rate professors and other students 
- **Reputation Management** – Prevents spam reviews and ensures fair rating calculations.  
- **Search & Filter** – Find users by name, course, or rating.  
- **Admin Moderation** – Tools to flag, review, and manage inappropriate content.

## OOP Principles Applied
## 1. Encapsulation  
- Secure sensitive user data (passwords, review content, permissions).  
- Private attributes with getter/setter methods for controlled access.  

## 2. Inheritance  
- **Base Class:** `User` (common attributes: name, email, role).  
- **Derived Classes:**  
  - `Student` (additional: enrolled courses, received ratings).  
  - `Professor` (additional: taught courses, received ratings).  
  - `Admin` (additional: moderation tools, reporting).  

## 3. Polymorphism  
- **Method Overloading:** Search function can take either a name, course, or rating range.  
- **Method Overriding:** Different user roles have distinct dashboard behaviors.  

## 4. Abstraction  
- **Interface:** `RateableEntity` with `submitReview()`.
- **Concrete Implementations:** `Student` and `Professor` implement the interface differently.  

## Technologies
- **GUI Framework:** React  
- **Database:** MongoDB  
