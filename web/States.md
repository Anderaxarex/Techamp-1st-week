|---------- Challenge prompt ----------|

This city never sleeps ♫

techcamp.jinblack.it:2007

|---------- Challenge solution ----------|

go to the address indicated in the challenge prompt
there are some tables on the databse, one of them is "us_states".
now by running a query like:

SELECT * FROM us_states WHERE name LIKE "%{%";

you will find an entry containing the flag

|---------- Challenge flag ----------|

flag{You_got_the_State_flag!}