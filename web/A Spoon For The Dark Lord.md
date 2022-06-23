|---------- Challenge prompt ----------|

We need a Spoon for Lord Voldemort! Please order one with his name on it. 
techcamp.jinblack.it:2010

|---------- Challenge solution ----------|

go to the address indicated in the challenge prompt
when you click on one of the links on the page there will be a form,  using the ispector you are able to notice the js script which is used to control the input and blocks every request with the words "Voldemort" or "Riddle"

This script is executed locally, so we can use BurpSuite to intercept the message beetwen our system and the server.

Open BurpSuite and go to "proxy", then press "intercept" and "open in browser".

A chromium tab will be displayed, then complete the form with any string. Press enter, then go to the BurpSuite window and press "forward". 

In the console will appear the string "name=<name>"

Change the string to "name=Lord Voldemort" and press "forward"

Back to chromium to copy the flag.

|---------- Challenge flag ----------|

flag{check_in_the_client_are_useless}