
# Challenge
Alice is a fan of Mécanique. She has two vintage cars and often likes to parade around with her ancestral objects. <br>
The mission will be to obtain Alice password

## Walkthrough 

### Real website
In our simulated case, the attacker will try to obtain the password for 2ememain, a well-known website for selling second-hand items. <br> 
The attacker will attempt to clone the login page of the targeted website.

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/6bd84a36-b455-4a44-b165-185b2b9d4121)

### Fake website
For this simulation, we will not attempt to clone the entire website architecture but will focus solely on the login page. We can simply use the inspector tools to copy and paste the HTML and CSS content. Any JavaScript that causes issues can be removed. The page may not be an exact replica, but our goal here is to demonstrate a phishing methodology. If we want to clone an entire website, we can use tools like Goclone or the Social Engineering Toolkit.

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

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/44823f2d-21a5-4aba-bb45-aa9a25a82ca6)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/1b044da5-baba-40e7-b2c0-38326e62a0da)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/dc31f3e5-1811-44ea-beff-495c92cd0dbe)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/05e88749-9bde-4596-95af-9143ad07dd44)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/b63e9fb0-7e67-4005-a405-e4250baccb87)

![image](https://github.com/AyraStelmaszewski/Cheatsheet-Phising/assets/68444023/57c5fcb2-7501-4575-82df-31ef0d3f3ad5)
