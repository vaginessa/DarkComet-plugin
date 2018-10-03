# DarkComet-plugin
![darkcomet-rat](https://user-images.githubusercontent.com/43011806/46427243-961fb300-c749-11e8-890f-8d359d1fb834.png)

This plugin made for Green force soft on your hacker's USB.

So the best way to start off your guide would be to explain what you will be working with first. So I will give you a quick explanation of Darkcomet, what it is and how it works. Darkcomet is a Remote Access Trojan or Remote Administration Tool. it is used mainly to gain access of a victim's PC but there are many uses for a RAT, I will provide most of them.
	
  •	Ability to control and view screen
	
  •	File management (Upload, Execute, Download, etc)
	
  •	Shell Access (CMD)
	
  •	Computer Power Access (Power off, log off, etc)
	
  •	Host and Registry control
	
  •	Keystroke viewing and control
	
  •	Network Monitoring (Wifi, View local PC's, etc)
	
  •	Password access on Chrome, Firefox, Opera, Safari and IE
	
  •	Task Manager Access

Darkcomet can be used for malicious intent, or for a prank. Many cyber criminals use RAT's like darkcomet to steal and log passwords, credit cards and more. There is a whole marketplace behind RAT's, it's mostly around botnets but RAT's are in the business too. People can make lot's of money with bots, they can use them to DDoS and make a DDoS service, steal their passwords, make shops and sell their accounts, keylog and sell logs, then sell the bots in a bot shop and a lot more.

Requirements

Okay so to have this correctly setup you are going to need a few simple requirements, I will list them below.
	
  1	Access to portforwarding (Your Router user and pass)
	
  2	Darkcomet 
	
  3	No-ip / DUC 
	
  4	Winrar or 7Zip


Tutorial

Okay so once you got all of the requirements and are ready to proceed, continue to this step by step tutorial and I will show you everything you need to know!

Darkcomet - Section 1

Installing, setting up and preparing Darkcomet - Darkcomet Section 1.1

1. Extract the darkcomet folder (VERY IMPORTANT)

2. Open Darkcomet.exe

3. Agree to the EULA, terms, etc

Portforwarding - Section 1

Okay so like I said, you need access to your router, otherwise you won't be able to portforward. You could still use an HTTP rat like "Loki Rat" if you don't want to portforward. Although if you want to go through all that trouble uploading the files to your FTP server and all that, you might as well go with an HTTP botnet like Cythosia, but let's get started.

Finding your Router Gateway Address - Portforwarding Section 1.1

1. Open your start menu

2. Search for "CMD" or Open "RUN" and type "CMD" on it.

3. Enter this code into your Command Prompt: "ipconfig"

4. Scroll all the way up and look for "Default Gateway" and "IPv4 Address"
(We will need IPv4 Address later)

Forwarding your Port - Portforwarding Section 1.2

5. Enter the Default Gateway IP into your URL bar

6. Login to your router, if you don't know your account search for some default logins.

7. Look for a portforwarding section (Might be in a gaming tab, every router is different)

8. Type "1604" on both "Starting Port" and "Ending Port"

9. For "Protocol" try "Both" but if there's only TCP and UDP, do both seperately

10. For "IP Address" get your IPv4 Address and enter it there

11. Enable the port and press submit

Allowing Port through Firewall - Portforwarding Section 1.3

1. Open Start menu and search "Firewall"

2. Click "Windows Firewall with Advance Security"

3. Go to "Incoming Connections" and click "New Rule"

4. Select "Port" and press the next button

5. Choose "UDP" and select "Specific Local Ports" and enter "1604"

6. Allow the connection and press next until you get to "Name"

7. Name is "darkcomet" or whatever, and give it any description

8. Click Finish and repeat it again for inbound connection but with "TCP" Port.

9. Repeat steps 1-8 but with "Outbound Connection"

10. Also you should check with your Antivirus firewall just in case.[/b]

Darkcomet - Section 2

Connecting and configuring Darkcomet - Darkcomet Section 2.1

1. Open Darkcomet.exe

2. Go to Socket / Net Section

3. Right click and press "Add port to listen to"

4. Make the Listen Port "1604" and enable "UPnP"

5. Click Listen and you have configured Darkcomet

Creating A Server (Stub/Virus) - Darkcomet Section 2.2

Okay now you will be making the virus that you will get users to run in order to infect them, there are many features on Darkcomet so I will take you through them.

1. Open Darkcomet Menu on top right corner

2 Go to Server Module and click Expert.
(If you want a list of what all the features do, read below)

Main Settings

Security Password - Adds a password so only you can manage bots
Mutex - Stops multiple connections on the same port
Server ID - The ID or Group bots that run this server are in
Profile Name - You can save your settings under a profile name
Process Hijacking - Firewall Bypass, not recommended if crypting (outdated)

Network Settings

IP/DNS - The DNS or IP Address bots will connect to
Port - Port bots will use to connect
Add - This will add the settings, remember to click this!
Also remember to click the added setting once added

Module Startup

Startup - Starts the stub with windows
Drop File in - Where the virus will be placed
Melt File - Deletes the virus execution file, but keeps virus after running
Date Created - Change the creation date to trick users
Persistence - Very important, keeps the program task from being removed

Install Message

This is basically where you make a fake error message when your virus starts to make it seem more legitimate.
Icon - Choose which img comes with the error, I suggest the "X" icon.
Title - What it says at the top of the error message (I.E "Error 804")
Message - What the actual error says "Warning, an unexpected error has occurred, program will now be terminated"
Test Messagebox - You can test the error on yourself, it is harmless and you can do it just to be sure

Module Shield

Persistent Process - Again, persistence for more than task manager, recommended.
EVERYTHING ELSE IF NOT RECOMMENDED AND IS OUTDATED IN THE MODULE SHIELD SECTION

Keylogger, Hosts, Binder, and Icon

Keylogger is able to send logged keys to a website through FTP connection.
You can manage a victim's "Hosts.txt" file through here and control which websites he can go on.
Bind a file with your server so they both run at the same time, this will make the user less suspicious.
Change icon of file to make it more legitimate and cause less suspicion.

DUC / No-iP - DNS Config Section 1

Creating a No-IP Account - DNS Config Section 1.1

1. Go to http://www.noip.com/newUser.php and register

2. Create a "No-ip.biz" hostname with any name you want

3. Click "No thanks, I'll use no-ip.biz" and click "Sign Up"

4. Validate your Email and Activate your Account

Configuring DUC - DNS Config Section 1.2

1. Open No/IP DUC and log into your No/Ip Account

2. Click "Edit Hosts" on the DUC Menu

3. Select your no-ip.biz website and click "Save"

4. Click Refresh Now and you're good to go!

5. Click File>Hide to get all of that out of your way

Setting up DUC or No/IP with Darkcomet - DNS Config Section 1.3

1. Open Dark Comet and click the drop down menu (Top right corner)

2. Click Server Module > Full Editor (Expert)

3. Use the Previous tips to setup your stub but leave the "Network Settings" alone

4. Instead of your IP address, enter your No/IP Website (DNS) and port "1604"

5. Press the "Add" button and click on it to select it

6. Finish your settings and press build stub

Tips and Tricks

Spreading

Spreading is basically a method to sending your server (virus) to a bunch of victims. This can be done best through a "Niche" which is basically a topic that a large amount of people are interested in, for example "Minecraft". You can make a Youtube Video about a "Minecraft Mass LastLogin Stealer" or something of the sorts, and spread your server. You can also do JDB's (Java Drive By) and use things like "Adult Cams" to attract and infect pedo's and pervs.

Crypting

Always be sure to crypt your file, this is when you edit the code of your virus to make it undectable (FUD) by antiviruses, this will durastically increase your spreading rates. You can buy a crypter from HF, use free ones or try using tools like obfuscation or hex editing to crypt it yourself. Always remember not to upload to av scanning websites that distribute your file otherwise it will become less UD, do NOT use "Virustotal" or "Novirusthanks". Instead you should use "Element Scanner". The best website to upload to would be: http://ge.tt

Money

You can make money through your bots in a lot of ways, so I will explain some of them.

1. Steal passwords and sell accounts

2. Bitcoin/Litecoin Mining

3. Sell DDoS service

4. Keylog and sell logs

5. Sell the bots themselves

(Be creative, these were just the ways i could think off the top of my head)
That is it for my tutorial for now, I hope you enjoy and thank you for reading. Please give me feedback on what you thought about this and how I should improve it, 

thanks!
