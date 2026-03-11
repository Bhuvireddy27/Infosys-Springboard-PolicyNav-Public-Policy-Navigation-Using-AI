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

SCREENSHOTS:
<img width="2560" height="1415" alt="Screenshot (104)" src="https://github.com/user-attachments/assets/0419746d-3ed4-4fb1-aead-e0342c8eb838" />
<img width="2560" height="1444" alt="Screenshot (103)" src="https://github.com/user-attachments/assets/15a80c46-6d02-4e52-8be0-4b65ef3d60ce" />
<img width="2560" height="1423" alt="Screenshot (102)" src="https://github.com/user-attachments/assets/40706470-c8c0-4108-8eca-c0aafd5cfe92" />
<img width="2560" height="1398" alt="Screenshot (101)" src="https://github.com/user-attachments/assets/ca3eb4a5-f124-41a0-8e78-c31647fb27d8" />
<img width="2560" height="1416" alt="Screenshot (107)" src="https://github.com/user-attachments/assets/8ad9ab57-52db-4ab8-b4a9-bbe73ae29fb8" />
<img width="2560" height="1407" alt="Screenshot (106)" src="https://github.com/user-attachments/assets/66a80df9-449c-49ca-96de-8d871f8a2585" />
<img width="2560" height="1406" alt="Screenshot (105)" src="https://github.com/user-attachments/assets/4a5eb818-94f9-46f3-a7f3-c4e6d57d160d" />
