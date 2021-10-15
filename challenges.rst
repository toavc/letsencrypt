Challenges
==================
To receive a certificate from Let’s Encrypt certificate authority (CA), you must pass a challenge to prove you control each of the domain names that will be listed in the certificate. A challenge is one of a list of specified tasks that only someone who controls the domain should be able to accomplish, such as:

Posting a specified file in a specified location on a web site (the HTTP-01 challenge)
Posting a specified DNS record in the domain name system (the DNS-01 challenge)
It’s possible to complete each type of challenge automatically (Certbot directly makes the necessary changes itself, or runs another program that does so), or manually (Certbot tells you to make a certain change, and you edit a configuration file of some kind in order to accomplish it). Certbot’s design favors performing challenges automatically, and this is the normal case for most users of Certbot.