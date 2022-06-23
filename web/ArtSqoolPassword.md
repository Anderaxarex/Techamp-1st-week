|---------- Challenge prompt ----------|

get the password of user admin 
techcamp.jinblack.it:2005

|---------- Challenge solution ----------|

go to the address indicated in the challenge prompt
log in with the admin user like you did for the "Art Sqool" challenge
now click on one of the links that are present and look at the url:

[http://techcamp.jinblack.it:2005/art?id=2]

Its pretty clear that the injection point is the "id" parameter. Now, we can use
a UNION to show the admin password. when using a union however, we must have the same number of selected elements on both sides. we want just one, so we can put a NULL to stand in for the other fields we should insert.

we got a hint of what the name of the field is from the login form. "Username" and "Password" with capital starters.
using your SQL skills, you should be able to find the password.

|---------- Challenge flag ----------|

flag{whooo_you_got_the_password_of_the_Admin!}