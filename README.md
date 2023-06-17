# BravePotato
SeImpersonatePrivilege Abuse. 
Ferramenta para abuso do privilégio SeImpersonatePrivilege.

I created this tool for the abuse of SeImpersonatePrivilege on any windows system since current tools are limited up to windows 10 on a specific build.

In general the idea is that you host a reverse shell (preferably created with msfvenom) somewhere and run this tool which will download your reverse shell and run it giving you back the shell with the "NT AUTHORITY\SYSTEM" account privilege  regardless of your current privilege level. 
The only prerequisite here is that your user has the "SeImpersonatePrivilege" privilege, you can check if this is possible with the simple command "whoami /priv".

It works together with the application created by Lee Christensen (https://github.com/leechristensen/SpoolSample) which has a copy already compiled right here in this directory.

How to use?
A picture is worth a thousand words: 



