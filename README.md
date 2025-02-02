# Email Sender Script

This repository contains a Python script for sending emails using the `smtplib` module.

## Features
- **Send Emails via SMTP**: Connects to an SMTP server to send emails.
- **Customizable Email Details**: Set sender, recipient, subject, and content.
- **Secure Connection**: Uses TLS encryption for secure email transmission.

## Prerequisites
- Python 3.x
- A Gmail account (or another SMTP-compatible email service)

## Installation
1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```
2. No additional dependencies are required beyond Python's built-in libraries.

## Usage
1. Modify the script to include your email credentials:
   ```python
   email['from'] = 'Your Name'   # Enter your name
   email['to'] = 'recipient@gmail.com' # Enter recipient's email
   email['subject'] = 'Your Subject' # Enter email subject

   email.set_content('Your email message')

   smtp.login('your-email@gmail.com', 'your-password') # Enter your email and password
   ```
2. Run the script:
   ```sh
   python email_sender.py
   ```
3. If successful, the script will print:
   ```
   all good mah boi!
   ```

## Notes
- **Security Warning**: Hardcoding your email and password is not recommended. Use environment variables or a secure authentication method.
- **App Passwords**: If using Gmail, enable "Less Secure Apps" or generate an App Password for authentication.
- **SMTP Configuration**: The script is set up for Gmail (`smtp.gmail.com`, port `587`). Modify for other email providers if needed.

## License
This project is licensed under the MIT License.

