# SECURITY-bank-app
Overview
This project implements a secure banking application backend using FastAPI with robust authentication and security measures. It demonstrates modern API security best practices for financial applications.

Key Features
Security Implementations:
1. Password Hashing: Uses bcrypt via passlib for secure password storage with salt
2. JWT Authentication: Token-based login system with expiration
3. Input Validation: Leverages Pydantic models for type-safe data handling
4. Protection Against Attacks: Defends against rainbow tables via salted hashing
5. No Plaintext Passwords: Ensures passwords are never stored or transmitted in clear text
6. Token Security: Implements token expiration and scoping

Core Functionality
1. User registration with email validation.
2. Secure login system generating JWT tokens
3. Account balance viewing
4. Deposit functionality with amount validation
5. Protected endpoints requiring valid JWT tokens

Technical Stack
1. Backend Framework: FastAPI (Python)
2. Authentication: OAuth2 with JWT tokens
3. Security Libraries: python-jose, passlib[bcrypt]
4. Development Tools: ngrok for secure HTTPS tunneling during testing
5. Validation: Pydantic models with email validation

Usage
The API provides endpoints for:
1. user registration (/register)
2. Login to obtain JWT token (/token)
3. View account details (/account)
4. Make deposits (/deposit)

Security Considerations
This implementation focuses on security best practices including:
1. Proper password storage (hashed and salted)
2. Secure token handling
3. Input validation
4. HTTPS communication (via ngrok in testing)
5. Protection against common web vulnerabilities

The project serves as a demonstration of how to build secure financial APIs while maintaining good development practices.
