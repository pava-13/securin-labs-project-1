# securin-labs-project
Secure Mini Payment API
📌 Project Overview

This project is a Secure Mini Payment Backend Service developed as part of an internship assessment. The system simulates a simplified payment environment where users can register, log in, perform payments, and view their transaction history.

The focus of this project is on secure backend design, authentication, and safe transaction processing.

🧠 My Approach

I designed the system using a structured backend architecture where:

User authentication is handled securely using password hashing.

Token-based authentication is used to protect sensitive endpoints.

Payments are validated before processing.

Each transaction is stored and linked to a specific user.

I focused on separating authentication logic, payment logic, and transaction handling to keep the code modular and maintainable.

⚙️ Tech Stack

Python

Flask (Backend framework)

SQLite / In-memory storage (based on your implementation)

Werkzeug (for password hashing)

JWT / Session-based authentication (mention what YOU used)

🔐 Security Considerations Implemented
1️⃣ Password Security

Passwords are hashed using a secure hashing algorithm.

Plain text passwords are never stored.

2️⃣ Authentication Protection

Token-based authentication is required for protected endpoints.

Token/session expiration implemented (if you did).

3️⃣ Input Validation

All input fields (email, password, amount, currency) are validated.

Basic protection against injection attacks.

4️⃣ Duplicate Payment Prevention

Implemented logic to prevent duplicate payment submissions.

5️⃣ Security Logging

Failed login attempts are logged.

Invalid token usage is tracked.

Suspicious payment attempts are monitored.

🛠️ API Endpoints
🔹 POST /register

Registers a new user.

Prevents duplicate email registration.

Stores hashed password.

🔹 POST /login

Authenticates user and generates token/session.

🔹 POST /payment

Processes payment.

Requires authentication.

Stores transaction securely.

Prevents duplicate submission.

🔹 GET /transactions

Returns transaction history of logged-in user only.

🚨 Threats Considered

While developing this project, I considered:

SQL Injection

Brute-force login attempts

Token misuse

Duplicate payment attacks

Unauthorized transaction access

🔍 What I Would Improve With More Time

Implement advanced rate limiting

Add idempotency keys for stronger duplicate prevention

Add role-based access control

Implement advanced logging & monitoring

Add automated testing

📂 Assumptions

Single-server environment

Not production deployed

Simple database used for simulation

🎯 IMPORTANT

Make sure:

You slightly adjust based on what YOU actually implemented.

Don’t claim features you didn’t build.

Keep language natural (not too perfect, not too robotic).
