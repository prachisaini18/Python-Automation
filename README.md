# Python-Automation

#send email using python 

**method 1**
steps:
#1. Importing the Necessary Libraries
#2. Establishing an SMTP Connection
#3. Logging into Your Gmail Account
#4. Composing the Email
#5. Sending the Email
#6. Closing the Connection

import smtplib
import pywhatkit
import os

server= smtplib.SMTP('smtp.gmail.com', 587)
server.starttls()
server.login('prachisaini2818@gmail.com', 'edha elcp **** ****')
message=input("enter your message to send: ")
server.sendmail('prachisaini2818@gmail.com', 'prachi1808saini@gmail.com', message)
print("success")
server.quit()


**method 2**
pywhatkit.send_mail(
    'prachisaini2818@gmail.com',
    'edha elcp dmfd nnpu',
    'Hello',
    'Hello from python',
    'prachi1808saini@gmail.com'
)
