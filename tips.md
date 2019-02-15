# Tips to help you get ready for the interviews:

1. Know how to intercept requests using Burp Suite Community Edition

2. Set up a *separate Chrome profile* in case you are on a live pentesting call sharing your screen with an interviewer. You do not want to intercept the call and embarrass yourself!
Bugcrowd a bugbounty platform has a great tutorial for setting up a separate Chrome profile
to prevent yourself from intercepting a call:
[Bugcrowd Chrome profile setup tutorial link here](https://youtu.be/h2duGBZLEek)

3. Know about HTTP status codes and their meaning! Status codes such as 500 can help you explain to an interviewer why you might actually be onto a serious bug such as SQLi. Here are a few status code responses:

- 200 OK means the request was successful 
- 301 Moved Permanently redirects browser to a different URL 
- 400 Bad Request user submitted a invalid HTTP request
- 500 Internal Server Error submitting unexpected user input

4. Know some basics on the Chrome/Mozilla Developer tools. This can really help with live web application pentesting interviews! 

5. Know the Same Origin Policy in depth. Why it works, how it can be bypassed, how does it come into play with state changing CSRF attacks. 

6. Know how CORS works and the process from the client all the way to the server side of how it is executed.

7. Be familiar reading code (Python) so you do not get stuck understanding a for loop iterating through each element in an array etc!

8. Create a profile on StackOverflow and GitHub and upload your own sample code to talk about during interview

