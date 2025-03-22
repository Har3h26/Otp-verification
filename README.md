
# **OTP Verification Using Python and Email**  

## **Overview**  
This project demonstrates how to implement **OTP (One-Time Password) verification** using **Python** and **email (SMTP)**. OTP verification is a common security measure used to authenticate users and protect sensitive operations.  

## **Features**  
✅ Generates a secure random OTP  
✅ Sends OTP to a specified email using SMTP  
✅ Validates user input against the generated OTP  
✅ Customizable OTP length and email format  
✅ Enhances authentication security in applications  

## **Prerequisites**  
Ensure you have the following before running the project:  
- **Python 3.6 or later**  
- **An SMTP server** (Gmail, Outlook, or any other provider)  
- **Email account credentials** to send OTPs  

## **Configuration**  
Before running the script, update your **SMTP settings** in `config.py`:  
```python
# SMTP server configuration  
SMTP_SERVER = 'your_smtp_server_host'  
SMTP_PORT = your_smtp_server_port  
SMTP_USERNAME = 'your_email@example.com'  
SMTP_PASSWORD = 'your_email_password'  
```  
Update sender and recipient email addresses in `otp_verification.py`:  
```python
sender_email = 'your_sender_email@example.com'  
receiver_email = 'your_recipient_email@example.com'  
```  

## **Usage**  
1. **Run the OTP verification script:**  
   ```sh
   python otp_verification.py  
   ```  
2. **Check your email** for the OTP.  
3. **Enter the OTP** when prompted.  
4. **Verification Result:**  
   - ✅ If correct, you’ll see a success message.  
   - ❌ If incorrect, you’ll be prompted to retry.  

## **Customization**  
Modify the `otp_verification.py` file for:  
- **OTP Length**: Change the `otp_length` variable.  
- **Email Subject & Content**: Edit `email_subject` and `email_body`.  
- **Expiration Time** (if added): Set a timeout for OTP validity.  

## **Security Considerations**  
- **Use environment variables** to store email credentials instead of hardcoding them.  
- **Enable two-factor authentication (2FA)** for your email provider and generate an **app password** instead of using your actual password.  
- **Use HTTPS connections** when integrating with web applications.  
