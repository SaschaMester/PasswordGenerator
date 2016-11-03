This is a password generator, based on a 
[Shellscript](https://jxself.org/password-generator.shtml) by [Jason 
Self](https://jxself.org/).  
  
Instead of using a password manager to store your passwords, this 
eliminates the need to store passwords entirely.  
  
Just make up a salt which you keep to yourself and use each time while 
combining it with some other value that's specific to the 
site/server/email account in question, like the domain name or email 
address or whatever.  
  
In this version your salt and site-specific thing are concatenated 
together, hashed, and then base64-encoded. The first 32 characters are 
returned as the password.  
  
Since the hashed value of your salt and that site-specific thing will 
always be unique you get a different password for each place. You also 
need never fear the loss or corruption of your password database, have 
to deal with backing it up, etc. since there isn't one. You can also 
always regenerate your passwords from anywhere using standard programs.  
  

The issue on the original Shellscript, linked above, was, that on the 
one hand, the salt won't be shown, but on the other hand, the string 
(e.g., the password) would be shown while typing.  
  
As Jason Self writes on the origin site of the script, linked above, he 
waives all copyright and related or neighboring rights to the script and 
applies the [Creative Commons Zero, 
CC0](http://creativecommons.org/publicdomain/zero/1.0/) to the script. 
The origin work is published from the United States.

The improvement (the string, e.g., the Password won't be shown anymore 
just by typing) was made by Sascha Mester on November 3rd of 2016.


