# CyberShield Security Web Application

A Flask-based cybersecurity testing web application designed for penetration testing practice. This application provides a secure environment for security professionals to test common web vulnerabilities in a controlled setting.

## Features

- User authentication system (login/signup)
- Secure password hashing with Werkzeug
- SQLite database for user management
- Responsive web design with cybersecurity theme
- Dedicated tools section with links to real cybersecurity tools
- Practice environment for penetration testing

## Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Git

## Installation Guide

### For Windows Users

1. **Install Python**
   - Download Python from [python.org](https://www.python.org/downloads/)
   - During installation, check "Add Python to PATH"
   - Verify installation: Open Command Prompt and type `python --version`

2. **Clone the Repository**
   ```cmd
   git clone https://github.com/yourusername/cybershield-app.git
   cd cybershield-app
   ```

3. **Create a Virtual Environment**
   ```cmd
   python -m venv venv
   venv\Scripts\activate
   ```

4. **Install Dependencies**
   ```cmd
   pip install -r requirements.txt
   ```

5. **Run the Application**
   ```cmd
   python app.py
   ```

6. **Access the Application**
   - Open your browser and go to `http://localhost:5000`
   - Use demo credentials:
     - Username: `admin`
     - Password: `password123`

### For Linux Users

1. **Install Python and pip**
   ```bash
   sudo apt update
   sudo apt install python3 python3-pip python3-venv
   ```

2. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/cybershield-app.git
   cd cybershield-app
   ```

3. **Create a Virtual Environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

4. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Application**
   ```bash
   python app.py
   ```

6. **Access the Application**
   - Open your browser and go to `http://localhost:5000`
   - Use demo credentials:
     - Username: `admin`
     - Password: `password123`

## Project Structure

```
cybershield-app/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # This file
├── static/
│   └── style.css         # CSS styles
└── templates/
    ├── base.html         # Base template
    ├── home.html         # Home page
    ├── login.html        # Login page
    └── signup.html       # Signup page
```

## Security Testing Guide

This application is designed for cybersecurity testing practice. Below are some areas you can test:

### 1. Authentication Testing
- Test for SQL injection in login forms
- Check for session management vulnerabilities
- Test for weak password policies
- Verify proper access controls

### 2. Input Validation Testing
- Test for XSS vulnerabilities in form inputs
- Check for CSRF protection
- Test for parameter tampering

### 3. Database Security
- Test for SQL injection vulnerabilities
- Check for sensitive data exposure
- Verify proper error handling

### 4. Session Management
- Test for session fixation
- Check for secure cookie attributes
- Verify proper logout functionality

### Important Notes for Testers

1. **This is a test application** - Do not use real personal information
2. **Designed for educational purposes** - Use only in controlled environments
3. **No real data protection** - This app doesn't have production-level security
4. **Test responsibly** - Only test on your own local installation

## Common Vulnerabilities to Test

- SQL Injection in login form
- Cross-Site Scripting (XSS) in user registration
- Cross-Site Request Forgery (CSRF)
- Session management flaws
- insecure direct object references

## Tools Integration

The application includes links to popular cybersecurity tools:
- **Reconnaissance**: Nmap, Amass, theHarvester
- **Vulnerability Scanners**: Nessus, OpenVAS, Nexpose
- **Web Application Testing**: Burp Suite, OWASP ZAP, Acunetix
- **Network Analysis**: Wireshark, Tcpdump, Npcap

## Troubleshooting

### Common Issues

1. **Port already in use**
   ```bash
   # Find process using port 5000
   lsof -i :5000
   # Kill the process or use a different port
   python app.py --port 5001
   ```

2. **Module not found errors**
   ```bash
   # Ensure virtual environment is activated
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   # Reinstall requirements
   pip install -r requirements.txt
   ```

3. **Database errors**
   ```bash
   # Delete the existing database file
   rm users.db
   # Restart the application to recreate it
   python app.py
   ```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## Disclaimer

This application is created for educational purposes only. Use it responsibly and only in environments where you have permission to perform security testing. The authors are not responsible for any misuse of this application.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For issues and questions:
1. Check the troubleshooting section above
2. Review existing GitHub issues
3. Create a new issue with detailed information about your problem

---

**Happy Testing!** Remember to always practice ethical hacking and only test systems you own or have permission to test.
