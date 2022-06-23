|---------- Challenge prompt ----------|

login as admin 
techcamp.jinblack.it:2005

|---------- Challenge solution ----------|

go to the address indicated in the challenge prompt
now put the Username field as "admin", and then use a SQL Injection
it should look like this:
Username [admin]
Password [' OR '1' = '1'; -- ]
remember to include a space both before and after the hyphon (-)

|---------- Challenge flag ----------|

flag{nice_you_managed_to_login_as_an_admin!}