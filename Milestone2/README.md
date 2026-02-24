Project Title

PolicyNav- Public Policy Navigation Using AI

Overview

Milestone 2 extends the secure authentication system developed in Milestone 1 by integrating:

- OTP-based password reset using Email
- JWT-secured OTP validation
- Login rate limiting
- Password history & reuse prevention
- Admin dashboard for user management
- Readability Analytics Dashboard
- Improved UI/UX with Neon Theme
- Secure environment-based secret management

This milestone focuses on security enhancement, analytics implementation, and UI improvement.

Features Implemented:

1. Advanced Authentication System:

- User Registration with password strength validation
- Secure Login with bcrypt hashing
- Login rate limiting (3 attempts lockout)
- Account auto-unlock after timeout
- Secure logout functionality
- Auto-created Admin account
- Password history tracking
- Prevent reuse of previous passwords


2. OTP-Based Password Reset System:

- OTP generated using HMAC-based algorithm
- OTP sent via Gmail SMTP server
- OTP stored securely using JWT (HS256)
- OTP expiration: 10 minutes
- Secure OTP verification
- Prevents reuse of old passwords
- Multi-stage reset flow (Email → OTP → Reset)

Security Flow:
1. User enters registered email
2. System generates OTP
3. OTP sent to email
4. OTP verified using JWT token
5. User resets password securely

3. Readability Dashboard:

A dedicated analytics dashboard that evaluates user-entered text.

It calculates:

- Total Word Count
- Sentence Count
- Average Sentence Length
- Estimated Readability Level
- Text Complexity Classification

Purpose:
- Demonstrates basic NLP techniques
- Provides user-friendly analytics visualization
- Adds data intelligence to the system

4. Admin Dashboard:

Admin Features:
- View all registered users
- See account creation timestamps
- Delete users (Admin protected)
- Admin account cannot be deleted

This ensures administrative control over system users.


Technologies Used:

- Python
- Streamlit
- SQLite3
- bcrypt
- PyJWT
- SMTP (Gmail)
- Pyngrok
- HMAC & Hashlib
- Regex Validation


 Algorithms Used:

- bcrypt hashing algorithm
- HMAC-SHA256 (JWT HS256 signing)
- HMAC-SHA1 (OTP generation logic)
- Regular Expressions for validation
- Heuristic readability scoring algorithm



Testing & Validation:

All modules were thoroughly tested:

✔ User Registration  
✔ Password Strength Validation  
✔ Login Success & Failure  
✔ Rate Limiting & Lockout  
✔ OTP Generation & Delivery  
✔ OTP Expiry Validation  
✔ Password Reuse Prevention  
✔ Admin User Deletion  
✔ Readability Score Accuracy  

All features are functioning correctly.


Steps to Run the Application (Google Colab)

Step 1: Install Dependencies
!pip install streamlit pyjwt bcrypt python-dotenv pyngrok -q
