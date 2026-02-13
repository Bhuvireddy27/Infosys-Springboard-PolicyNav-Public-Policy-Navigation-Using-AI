Milestone 1 – User Authentication System

PolicyNav – Public Policy Navigation Using AI

Description: Milestone 1 focuses on designing and implementing a secure user authentication system for the PolicyNav application.  
This authentication module serves as the foundation for future AI-based features such as policy search, analysis, and summarization.

The system includes user registration, secure login, password recovery, and session handling, implemented with best security practices.

Features Implemented:
- User Signup with:
  - Mandatory field validation
  - Valid email format validation
  - Alphanumeric password enforcement
  - Security question and answer
- Secure Login:
  - Case-insensitive email handling
  - Password verification using hashing
- Forgot Password:
  - Email existence verification
  - Security question–based authentication
  - Case-insensitive security answer matching
  - New password and confirm password validation
  - Prevention of old password reuse
- Dashboard:
  - Welcome message after successful login
- Secure password storage using hashing
- Streamlit-based interactive UI
- Ngrok integration for public access (for demo)

Technologies Used:
- Python 3.12 (Google Colab runtime)
- Streamlit Frontend UI
- SQLite – Database for user credentials
- bcrypt – Secure password hashing
- JWT (PyJWT) – Authentication token handling
- Ngrok – Public URL exposure

Steps to Run the Application (Google Colab)

1. Open Google Colab.
2. Upload all project files
3. Install required dependencies:
   pip install streamlit pyjwt bcrypt pyngrok
4. Run the Streamlit application:  
    streamlit run app.py
5. Use ngrok to expose the application:
    from pyngrok import ngrok
    ngrok.set_auth_token("YOUR_NGROK_AUTHTOKEN")
    public_url = ngrok.connect(8501)
    print(public_url)

ScreenShots:
SIGN-UP PAGE-
 <img width="2559" height="1334" alt="Screenshot 2026-02-13 224855" src="https://github.com/user-attachments/assets/c4eac3ab-6a0e-4375-9cb3-dc59ffe8c6ec" />
LOGIN PAGE-
<img width="2559" height="1330" alt="Screenshot 2026-02-13 225022" src="https://github.com/user-attachments/assets/3992965f-2baf-435f-bb53-080dd69818df" />
DASHBOARD-
<img width="2559" height="1417" alt="Screenshot 2026-02-13 232254" src="https://github.com/user-attachments/assets/848ee3ee-4a48-440b-bafe-192917100da9" />
FORGOT PASSSWORD PAGE-
<img width="2559" height="1330" alt="Screenshot 2026-02-13 225310" src="https://github.com/user-attachments/assets/d22aa1a4-0df4-41e9-b100-e4509cfee9ec" />
