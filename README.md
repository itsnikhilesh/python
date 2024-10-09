# python
Project name :  News Headlines Console Screen with Login and API Integration

Project Title1: News Headlines Console Screen with Login and API Integration
Problem Statement:
Create a Python-based console application where users need to log in to access the top 5 news headlines based on a keyword of their choice. The user credentials should be stored in a CSV file, and a password reset option should be available. The application should limit tailed login attempts to prevent unauthorized access. Upon successful login, the app will fetch and display news headlines from NewsAPI.
Requirements:

1.Login System:

User credentials are stored in a CSV file (regno.csv). The file contains fields like email, password (hashed), and security_question (for password recovery).
During login, the system will prompt the user for their email and password.

2.Input Validation:

The email must be in a valid format (e.g., example@domain.com).
The password must meet a minimum length of 8 characters, contain at least one special character, and be validated against the stored password (use hashing for comparison).

3.Forgot Password:

If the user chooses to reset their password, they are prompted to enter their registered email.
If the email exists in the CSV file, the user must answer a security question correctly. Upon correct answer, they can set a new password.

4.Login Attempts:

The user is allowed up to 5 login attempts. After 5 failed attempts, the user is logged out, and further attempts are denied until the application restarts.

5.API Integration (NewsAPI):

After successful login, prompt the user to enter a keyword or topic of interest.
Use the NewsAPI to fetch the top 5 latest news headlines related to the keyword.
Display the headlines, along with the source, in the console.

6.Error Handling:

Handle cases where the API key is invalid or expired.
Handle network errors (e.g., no internet connection).
Handle cases where no news results are found for the given keyword.
