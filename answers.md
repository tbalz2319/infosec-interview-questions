 ```                                                       
  ,---.                                                  
 /  O  \ ,--,--,  ,---. ,--.   ,--. ,---. ,--.--. ,---.  
|  .-.  ||      \(  .-' |  |.'.|  || .-. :|  .--'(  .-'  
|  | |  ||  ||  |.-'  `)|   .'.   |\   --.|  |   .-'  `) 
`--' `--'`--''--'`----' '--'   '--' `----'`--'   `----'  
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
```
                                                                                      
**What can you assume if you are on a web application anf there
is a search bar which trows a HTTP status 500 error after you enter a ' in the search?**

I can begin to assume by entering ' in a search bar based on the 500 status code means the input I typed was received but the server encountered an error. So I would begin to assume I am onto a SQL bug and start sending in some SQL commands such as sleep(5) then wait to see if before I get a response the web page loads for about 5 seconds


**Are you familiar with some automated tools that can help you find
SQL Injectons? What are they called?**

I am familiar with some of the automation tools in Kali Linux for finding SQL injection points such as SQLMAP. 

**Do you know what XXE is, can you explain it?**

XXE stands for XML External Entities. It means attackers can upload XML files by to exploit the site's XML parser. User data or more serious attacks such as the Billion Laughs Dos attack can be triggered.

**Are you familiar with OWASP? Can you name some of the TOP 10 2017 vulnerabilities and explain what they are?**

OWASP stand for the Open Web Application Security Project, it's a community of people that provide free resources to the community on the topics of web application security. They are ost know for realising the OWASP TOP 10 vulnerabilities for each year. The OWASP Top 10 2017 is list of the top vulnerabilities most commonly found in web applications based on reports for multiple companies, agencies and researchers. 


**Can you explain the process of when I type google.com into the search bar then I get results back?**

**Can you explain what XSS is and the different types of XSS?**
XSS is Cross-Site Scripting a very common vulnerability where an attacker can execute malicious JavaScript code to 
compromise user data, sessions etc. The three different types of XSS are 

1) Reflected, this XSS is triggered once in the body of the request 
2) Stored, a Javascript payload is saved in the application's database and can be triggered multiple times until it is removed. Common places of where to find stored XSS attack is in user comments, profile bios, document uploads. 
3) DOM, the Document Object Model (DOM) is used to set malcious javascript

**What does it mean when cookies have an HttpOnly flag?**
The HttpOnly flag blocks attackers from using `document.cookie` to get the applications cookie
which is often used to steal user sessions and decrypt any other weakly encrypted data!

**What is Self-XSS an why is it not a vaid bug to report?**
Self-XSS is when a user has to pop open the Chrome/Mozilla Developer tools
and type in themselves a malicious JavaScript. This bug is often out of scope for bugbounty programs
as it requires an attacker to have to convice a user to self inflict themselves.

**What are some SQLi methods you can use if you are dealing with a blind SQL injection to confirm your query is executing?**
Using time-based queries to try and see if the query executes the delay can help an attacker determine whether or not they
are sucessfully injecting commands to the database. After they fingerprint what type of databse the application uses such as Oracle, MS-SQL, MySQL MongoDB and attacker can look up time-based commands for the corresponding database. For example for MySQL using sleep(10) will delay the reponse 
and for 10 seconds so the attacker can notice if their query is running.

**What is the SAME ORGIN policy?**
The SAME ORIGIN policy 

**What is CSRF and what are some ways to prevent it?**
CSRF stands for Cross-Site Request Forgery it is when an attacker leverages a user who is already authenthicated in a web application (i.e they already have an account and are logged in) to then trick the user into performing unwanted operations on the web application.
An example would be  