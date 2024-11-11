# A-Level Draughts Project

<!--ts-->
   * [Background Information](#background-information)
   * [Core Features](#core-features)
   * [Testing and Limitations](#testing-and-limitations)
   * [Running the program](#running-the-program)

<!--te-->

# Background Information

This project was made for my OCR A-Level NVQ Project and is a fully-functional version of Draughts with a user-friendly interface, complex database interactions and additional functionalities such as verifying emails through temporary passwords, which culminated in me earning an 'A' grade.

# Core Features

- Java has been used to implement the game logic and handle the mechanics of Draughts, using object-oriented programming principles and efficient coding practices, such as using ArrayLists for efficient storage and retrieval of ordered data. 
- Java Swing has been used to create the front-end views (menu, help, etc.) and the GUI for Draughts, using event-driven programming (event listeners/handlers) to ensure responsiveness and an ergonomic user experience while satisfying the stakeholder requests of being a relaxing, educational platform to play Draughts. 
- SQL is used to manage the database interactions, which consist of storing user data for logging in and keeping track of scores for leaderboards (although this wasn't fully implemented in time). As such, the database schema is designed with tables for user profiles, game records, and leaderboards, and are carefully defined using foreign keys and constraints to maintain data integrity. Furthermore, prepared statements are used to prevent SQL injection attacks, ensuring the security of user-database interactions.
- One additional functionality of the project was the validation and verification of new email addresses through a temporary auto-generated password. A method was implemented to generate a random 10-character password comprising alphanumeric characters and special symbols, ensuring security. The JavaMail API was then used to send the password to the provided email address, with an appropriate SMTP configuration (host: smtp.office365.com, port number: 587 for TLS encryption, authentication credentials: sender's email and password). The webmail provider used was Microsoft Outlook as it offers end-to-end encryption whereas other sites such as Gmail only encrypt emails while in transit [therefore providing an extra layer of security](https://www.contactmonkey.com/blog/outlook-vs-gmail-for-business-email#:~:text=Both%20services%20also%20offer%20different,employees%20stay%20alert%20and%20safe.).

# Testing and Limitations

Throughout the development process, various testing techniques have been used to ensure that the program meets the stakeholder's requirements, including:

- Unit Testing: JUnit was used to test individual methods and classes to ensure expected functioning and output.
- Integration Testing: This involved testing the interaction between different components of the system for errors and functionality.
- Black Box Testing: Evaluation of the usability and functionality of the program without knowledge of the underlying code was done to identify issues from the user's perspective.

However, there are some limitations to this project. Due to time and resource constraints, some features, such as accelerated game timers and additional accessibility options, were not able to be implemented. Additionally, the program's scalability on different screen sizes is an issue that needs to be addressed in further development. Furthermore, maintenance of the project is also important to ensure that the program remains up-to-date - for example, monitoring and incorporating changes from the JavaMail API community or Oracle updates - in order to maintain the application's reliability and security over time.

# Running the program

Although the final codebase was not able to be retrieved, the complete documentation of the analysis, design (pseudocode and UI/UX), development, and evaluation is available in the Word document.
