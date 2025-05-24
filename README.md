# Exercise-10-Email-Automation---send-email

~~~
Name : FRANKLIN.F  
Reg.No : 212224240041 
~~~

## Aim
To create a UiPath workflow that sends an email using a Gmail account through SMTP or Outlook activities.

## Materials Required

UiPath Studio
Gmail account
Internet connection
Mail Activities package (installed by default)
Enable "Less secure apps access" or App Passwords in Gmail settings (if 2FA is enabled)

## Procedure

Step 1: Setup Gmail for SMTP Access
Enable 2-Step Verification on your Gmail account.
Go to https://myaccount.google.com/apppasswords
Generate an App Password (e.g., for "Mail on Windows Computer"). 
Copy and save the app password securely — you’ll use it in UiPath.

Step 2: Create a New UiPath Process
Open UiPath Studio and create a new process named GmailSenderBot.

Step 3: Use Send SMTP Mail Message
Drag the Send SMTP Mail Message activity (found in UiPath.Mail.SMTP.Activities).

Fill in the properties:

Property	Value
To	"recipient@example.com"
Subject	"Test Email from UiPath"
Body	"Hello! This is a test email from UiPath automation."
Port	587
Server	"smtp.gmail.com"
Email	"your_email@gmail.com"
Password	Paste your Gmail App Password securely
SecureConnection	StartTls

Step 4: Run the Workflow
Save and run the bot.

The email will be sent to the recipient from your Gmail account.

## OUTPUT:
An email will be delivered to the recipient with the subject and message body specified.
![Screenshot 2025-05-12 090312](https://github.com/user-attachments/assets/17c09443-5eae-44ff-a074-6ff1bfc1edbd)

![Screenshot 2025-05-12 090358](https://github.com/user-attachments/assets/3373b9ee-358d-4f6a-97f3-7de74e15912f)

![image](https://github.com/user-attachments/assets/70f102fb-87e2-4574-b221-e7a6fcacbcea)


## Result:
The UiPath workflow successfully sends an email from a Gmail account using SMTP configuration.
