# Null-ActiveDirectory-Whitelistbypass
Contains all the references and code used in the session at Null. 

## How to install Active Directory?
https://medium.com/harsh-thakur/how-to-install-active-directory-663c685355ee

## How to gain credentials? 
https://hausec.com/2019/03/05/penetration-testing-active-directory-part-i/

## Using Crackmapexec to enumerate shares 
https://www.youtube.com/watch?v=ekgeVecQH94
https://www.youtube.com/watch?v=Dd4ZAm2mwwA&t=2191s

## Ways to remotely execute commands on Windows
https://blog.ropnop.com/using-credentials-to-own-windows-boxes-part-2-psexec-and-services/

# Common Application WhiteList Bypass Methods

## mshta 
C2 server : https://github.com/zerosum0x0/koadic to generate malicious html application and pass it to crackmapexec for remotely executing command on windows.

## wmic 
Code for POC can be found here: https://gist.github.com/mycryptonite/8d47f2ee6ca176ff732e367c8e201db0  
You can find weaponized versions of the code automatically generated by C2 frameworks like SilentTrinity: https://github.com/byt3bl33d3r/SILENTTRINITY

Read more about it in:
http://archive.is/subt0x10.blogspot.nl

## csc and InstallUtil
For CLRv2 i.e if you're compiling with v2.0.5 or less, then you can add this part as Uninstaller :
https://gist.github.com/mycryptonite/f2abdb2a9ad8d2d6ddaa5072ae7c175d 

For CLRv4, use this code. Creating a runspace avoids the exception of AccessViolation created using the previously mentioned snippet. Code: https://gist.github.com/mycryptonite/f2abdb2a9ad8d2d6ddaa5072ae7c175d

## regsvr32
You can find the POC code here:
https://gist.github.com/mycryptonite/3612e490fafd6c91d1a674b967752d4a

For detailed explanatioin, watch this:
https://www.youtube.com/watch?v=3gz1QmiMhss&t=661s

## Other references, techniques and interesting articles can be found here:
https://www.secureauth.com/blog/playing-relayed-credentials

https://www.microsoft.com/en-us/download/details.aspx?id=46899

https://www.blackhillsinfosec.com/evade-application-whitelisting-using-regsvr32/

https://byt3bl33d3r.github.io/author/byt3bl33d3r.html

https://hausec.com/

https://adsecurity.org/

https://cobbr.io/SharpSploit.html

https://www.hackingarticles.in/post-exploitation-using-wmic-system-command/

https://blog.conscioushacker.io/index.php/category/application-whitelisting/

https://enigma0x3.net/

http://archive.is/subt0x10.blogspot.nl

https://github.com/khr0x40sh/WhiteListEvasion

https://medium.com/@Bank_Security/undetectable-c-c-reverse-shells-fab4c0ec4f15

https://web.archive.org/web/20161214101107/http://thrysoee.dk/InsideCOM+/ch05e.htm

https://enigma0x3.net/2017/08/03/wsh-injection-a-case-study/
