|---------- Challenge prompt ----------|

There are so many cities O:

techcamp.jinblack.it:2007

|---------- Challenge solution ----------|

go to the address indicated in the challenge prompt
there are some tables on the databse, one of them is "us_cities".
now by running a query like:

select * from us_cities where city or county like "flag{%";

you will find an entry containing the flag

|---------- Challenge flag ----------|

flag{nice_you_got_also_the_city_flag!}