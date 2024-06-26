
# Challenge
Alice is a fan of Mécanique. She has two vintage cars and often likes to parade around with her ancestral objects. <br>
The mission will be to obtain Alice password

## Walkthrough 

### Real website
In our simulated case, the attacker will try to obtain the password for 2ememain, a well-known website for selling second-hand items. <br> 
The attacker will attempt to clone the login page of the targeted website.

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/6bd84a36-b455-4a44-b165-185b2b9d4121)

### Fake website
For this simulation, we will not attempt to clone the entire website architecture but will focus solely on the login page. We can simply use the inspector tools to copy and paste the HTML and CSS content. I'll remove any JavaScript that causes issues , the page may not be an exact replica, but our goal here is to demonstrate a phishing methodology. If we want to clone an entire website, we can use tools like Goclone or the Social Engineering Toolkit.

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/211cb0c4-b230-4148-8fbc-f8577d35dd52)

### Build a way to store the form data

#### Databases
An attacker could choose to build a database system to store the data. <br>
For this demonstration, we'll use a NoSQL database, MongoDB, which is straightforward to integrate into a Flask app.<br>
Of course, this controller could be improved with features like prefilled email fields, redirection to the real website, or even a redirection and connection with the stolen credentials. <br> 
However, we'll keep it simple with a blank form and no specific redirection except to the login page.

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/62fa94e3-1ab3-4aaf-ba56-370d88119280)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/da4e3c08-c4ac-4f4b-888e-3762cf44df49)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/e156242a-ffd5-41ef-95dd-dced4104aba6)


#### HTTP request
Our attacker could avoid creating a database and instead aim to obtain the credentials directly from the HTTP request when the form is submitted. <br>
To capture the data, we can simply set the "action" attribute in the form tag to redirect the submission to our server. <br> For this demonstration, we're using webhook.site, a free service that fits well for this purpose.

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/05e88749-9bde-4596-95af-9143ad07dd44)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/b63e9fb0-7e67-4005-a405-e4250baccb87)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/57c5fcb2-7501-4575-82df-31ef0d3f3ad5)

### Fake email

The attacker will need to use a coherent email address to send a malicious email with the goal of tricking the victim into clicking on a fake link. This is the principle of phishing. To achieve this, the attacker will need to spoof the style of an official email to make it look realistic and then create an email address that appears to be an official email from the targeted website. Just like with the login page, we can inspect and replicate the current email style. <br>

For the purpose of this demonstration, I created the email address no_reply_2ememain@fastmail.com. <br>
Fastmail is a free service that provides email addresses.
![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/1b044da5-baba-40e7-b2c0-38326e62a0da)
![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/dc31f3e5-1811-44ea-beff-495c92cd0dbe)

For the demonstration, I used one of my Google accounts with an actual history of emails from the copied service so we can compare our fake email with the official ones.
![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/44823f2d-21a5-4aba-bb45-aa9a25a82ca6)

### Conclusion 

Phishing remains one of the most pervasive and damaging cyber threats faced by individuals and organizations alike. This proof of concept (PoC) illustrates the simplicity with which attackers can mimic legitimate websites, deceive users into divulging sensitive information, and potentially wreak havoc on both personal and corporate security.

The techniques showcased here demonstrate how attackers can exploit the trust users place in familiar websites by crafting convincing replicas of login pages and emails. With just a few simple tools and minimal technical expertise, attackers can trick unsuspecting users into surrendering their credentials, opening the door to a range of malicious activities such as identity theft, financial fraud, and unauthorized access to sensitive data.

For large companies and organizations, the implications of phishing attacks are particularly grave. Not only do they risk compromising the personal information of their users, but they also face the threat of reputational damage, financial loss, and regulatory repercussions. Moreover, as seen in this PoC, even sophisticated security measures can be circumvented by attackers with relative ease.


