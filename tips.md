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

4. Know some basics on the Chrome/Mozilla Developer tools. Simple things such as knowing how to inspect an element change hidden attributes to visible can help! Below are some JS tips:

- Right click inspect
-  Changing attribute values of hidden inputs from hidden to display. This can sometimes popup interesting IDs or functionalities: 
    `<input  name="usrId" type="hidden" value="">`
- In the developer console typing: `document.cookie` to show the currently set cookies
- HTML comments are denoted by arrows `<!-- this is a comment -->` they can sometimes help reveal hidden content or verbose developer oopsies such as AWS keys

