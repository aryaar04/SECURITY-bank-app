# SECURITY-bank-app
Overview
This project implements a secure banking application backend using FastAPI with robust authentication and security measures. It demonstrates modern API security best practices for financial applications.

Key Features
Security Implementations
Password Hashing: Uses bcrypt via passlib for secure password storage with salt

JWT Authentication: Token-based login system with expiration

Input Validation: Leverages Pydantic models for type-safe data handling

Protection Against Attacks: Defends against rainbow tables via salted hashing

No Plaintext Passwords: Ensures passwords are never stored or transmitted in clear text

Token Security: Implements token expiration and scoping

Core Functionality
User registration with email validation

Secure login system generating JWT tokens

Account balance viewing

Deposit functionality with amount validation

Protected endpoints requiring valid JWT tokens

Technical Stack
Backend Framework: FastAPI (Python)

Authentication: OAuth2 with JWT tokens

Security Libraries: python-jose, passlib[bcrypt]

Development Tools: ngrok for secure HTTPS tunneling during testing

Validation: Pydantic models with email validation

Usage
The API provides endpoints for:

User registration (/register)

Login to obtain JWT token (/token)

View account details (/account)

Make deposits (/deposit)

Security Considerations
This implementation focuses on security best practices including:

Proper password storage (hashed and salted)

Secure token handling

Input validation

HTTPS communication (via ngrok in testing)

Protection against common web vulnerabilities

The project serves as a demonstration of how to build secure financial APIs while maintaining good development practices.
