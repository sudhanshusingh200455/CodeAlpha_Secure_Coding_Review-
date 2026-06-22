# Secure Coding Review

## Overview
This project was completed as part of the CodeAlpha Cyber Security Internship.

The objective of this project is to identify common security vulnerabilities in source code and recommend secure coding practices to improve application security.

## Vulnerability Reviewed
### SQL Injection

SQL Injection is a security vulnerability that allows attackers to manipulate database queries through user input.

## Vulnerable Code Example

username = input("Enter username: ")
query = "SELECT * FROM users WHERE username = '" + username + "'"

## Secure Code Example

username = input("Enter username: ")

cursor.execute(
    "SELECT * FROM users WHERE username = %s",
    (username,)
)

## Recommendations
- Validate all user inputs
- Use parameterized queries
- Implement proper error handling
- Store passwords securely
- Encrypt sensitive data

## Tools Used
- Microsoft Word
- PDF Documentation

## Conclusion
Secure coding practices help developers reduce vulnerabilities and protect applications from cyber threats.

## Author
Sudhanshu Singh

## Internship
CodeAlpha Cyber Security Internship
