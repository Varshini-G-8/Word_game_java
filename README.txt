WORD GUESS GAME — SIMPLE JAVA WEB APPLICATION

This version uses Java's built-in HTTP server. No Maven, Spring Boot, Tomcat,
database installation, or third-party libraries are required.

REQUIREMENTS
- JDK 11 or newer.

RUN ON WINDOWS
1. Extract the ZIP to a folder.
2. Open PowerShell in the WordGuessJavaSimple folder.
3. Check Java: java -version and javac -version
4. Compile: javac -encoding UTF-8 Main.java
5. Start: java Main
6. Open http://localhost:8080 in your browser.

FIRST-RUN ADMIN SETUP
- Open http://localhost:8080/admin/setup to create your own administrator account.
- Setup is available only until an administrator account exists.
- No default administrator username or password is printed or preconfigured.

FEATURES
- Browser-based UI using the original project's stylesheet and responsive layout
- Player registration and login
- Username validation (at least five letters)
- Password validation (at least five characters, a letter, a digit, and one of $ % *)
- Word guessing: five-letter words, five guesses, green/orange/grey feedback
- Three rounds per player per calendar day
- Admin dashboard, daily report, and per-player report
- Persistent storage in wordgame-data.ser, created automatically when the application runs
- Passwords are stored as PBKDF2 hashes

NOTES
- All project data is stored locally in wordgame-data.ser. Keep this file to retain users and reports.
- Keep Main.java, static/style.css, and wordgame-data.ser in the same working folder.
- Stop the server with Ctrl+C.
- Intended for local coursework/demo use, not public internet deployment.
