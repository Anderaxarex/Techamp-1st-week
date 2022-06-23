|---------- Challenge prompt ----------|

Retrieve the sourcecode of the application 
techcamp.jinblack.it:2004

|---------- Challenge solution ----------|

go to the address indicated in the challenge prompt
when you click on one of the links on the page, the url will change to something like:

[http://techcamp.jinblack.it:2004/gallery?category=ctf]

as is pretty clear, the category parameter is our traversal point. by traveling back two directories we will be at the root of the file system. We can see that there is onle one directory that is not usual: "/chall" if we put that as our new url, we can see two things: 
  art
  templates
  [unidentified]

if we inspect the unidentified object, we see that the src field in its html points to this route:
  [/img?img=../../chall/app.py]

if we put that after the url in the prompt, we are greeted by the source code of the application.

|---------- Challenge flag ----------|

flag{nice_you_did_a_path_traversal!!!}