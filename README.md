# 3DFii
NOTICE: This is **UNFINISHED** so please **DO NOT COMPLAIN** if it breaks on you.
<br>
Discord: https://discord.gg/3U3qxha

# How to Setup
Requirements:
<br>
Node.js
<br>
Fiddler4
<br>
Luma3DS Game Patching
<br>
Knowledge
<br>
*********************
<br>
Alright so lets jump right in!
<br>
<br>
Make sure you unlink your NNID before doing any of this.
<br>
<br>
Open up Fiddler4 and then go to Tools->Options->Connections then select "Allow Remote Computers" and restart Fiddler4.
<br>
<br>
Go to Tools->Options->Connections in Fiddler4 and select "Capture HTTPS CONNECTs" if its not already selected then select "Decrypt HTTPS traffic" DO NOT INSTALL ANY CERTIFICATES IT SAYS TO INSTALL JUST HIT NO I REPEAT **DO NOT INSTALL ANY CERTIFICATES IT SAYS TO INSTALL**.
<br>
<br>
Open Command Prompt and type ipconfig and find your local IP, you'll need this for later.
<br>
<br>
Go to 3DS Settings and go to Internet settings and select your WiFi that is going to be used for this and hit change settings then go to proxy settings and turn it on and then hit detailed setup and then enter your local IP from the last step into proxy server and port 8888 into port and let it do a connection test and hopefully it connected successfully.
<br>
<br>
Download this repository from here https://github.com/ProjectFii/3DFii/archive/master.zip and join the Discord and go to announcements and find the pack.zip in pinned messages and extract it somewhere.
<br>
<br>
Then move ClientCertificate.cer to Documents->Fiddler2 or Documents->Fiddler4 depending on what version and sometimes Fiddler4 uses the Fiddler2 folder.
<br>
<br>
Then move the titles folder to your luma folder on your SD card, make sure you have game patching enabled.
<br>
<br>
Then extract the OpenServices repository ZIP file somewhere and open command prompt and CD to it.
<br>
<br>
Do "npm install https express" in the root of the repository files and then cd to NNIDServices and run this "npm install fs path"
<br>
<br>
Then run "node NNIDService" and hopefully it should run just make sure you have no applications using port 80/443 and **its normal if you get nothing in command prompt**.
<br>
<br>
Go to Tools->HOSTS and enable it and type "(your local IP from command prompt) account.nintendo.net" and hit save.
<br>
<br>
Then finally restart Fiddler4 and turn on your 3DS and go to settings and register for a NNID and hopefully it should register just fine.
<br>
<br>
And to unregister simply turn off the proxy on your 3ds and login using a random password and hope that it will allow you to create a new account.

# Credits
SciresM - For 3DS SSL patch
<br>
If I forgot anybody else please hit me up on the Discord.
