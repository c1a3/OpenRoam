# OpenRoam
OpenRoam is a freeroam SA-MP server, a multiplayer mod for Grand Theft Auto San Andreas and with a working database. <br><br>
<b>SA-MP</b> (San Andreas Multiplayer) is a free, third-party multiplayer modification for the PC version of Grand Theft Auto: San Andreas.  It transforms the single-player game into a massively multiplayer online experience, allowing users to play against or with each other over the internet or LAN.

### Key Features
- <b>Massive Scale:</b> Servers can support up to 1,000 players simultaneously. 
- <b>Custom Game Modes:</b> Utilizing the PAWN scripting language, server owners can create diverse game modes ranging from Roleplay (RP) and Deathmatch to Racing and Capture the Flag. 
- <b>Requirements:</b> Players can use either a legitimate copy or even a pirated one, of the PC version of Grand Theft Auto: San Andreas to install and run the mod.

OpenRoam currently supports upto 50 players on freeroam.

Server Setup
----------------------

I have included both plugins for Windows and Linux servers, to set up a quick testing environment on your computer:

- Install XAMMP
- Start the Apache and MySQL server
- Open Phpmyadmin and create a new database
- Put the details of the database in your script
- Run the server


SA-MP 0.3 Server Setup
----------------------

Once the configuration is complete, run> ./samp03svr & to start the server process.

CONFIGURATION:

Example server.cfg:
	echo Executing Server Config...
	lanmode 0
	maxplayers 32
	port 7777
	hostname Unnamed Server
	announce 0
	gamemode0 lvdm 1
	gamemode1 rivershell 1
	weburl www.sa-mp.com
	rcon_password changeme

To configure the server, you must edit the values in server.cfg. They 
are explained below:

hostname
--------
	Parameters:
		string
	
	Description:
		Specifies the hostname shown in the server browser
		
port
----
	Parameters:
		int
	
	Description:
		Specifies the port to listen on.
		This port is used for game connections, rcon 
connections, and for querying.
	
maxplayers
----------
	Parameters:
		int
	
	Description:
		Specifies the maximum amount of players.
		
lanmode
-------
	Parameters:
		int (0 or 1)
		
	Description:
		Turns lanmode on (1) or off (0). Lanmode (as the name 
suggests) is for use on LAN games, where bandwidth is not a problem. 
Lanmode sends data at a higher rate, for a smoother game.
		

announce
-------
	Parameters:
		int (0 or 1)
		
	Description:
		Announces your server to the 'Internet' server list in 
the SA:MP browser. On (1) or Off (0).

weburl
------
	Parameters:
		string
	
	Description:
		Specifies the URL shown in the server browser, which is 
associated to the server.
		
rcon_password
-------------
	Parameters:
		string
		
	Description:
		Specifies the password needed to connect to rcon, or 
login to rcon ingame.
		
gamemode0 - gamemode15
----------------------
	Parameters:
		string
		int
		
	Description:
		Specifies the rotation settings. The first parameter 
sets the game mode name. The second is the number of times it will 
repeat.
		You can use gamemode0 to specify the first gamemode, 
gamemode1 to specify the second, etc.

## In-game Screenshots
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/c8f745ec-2524-4b46-8768-7c09a98789b9" />


## Dependencies  
| Name | Version | URL |
| --------------- | --------------- | --------------- |
| MySQL Plugins | R41-4 | [https://github.com/pBlueG/SA-MP-MySQL/releases/tag/R41-4](https://github.com/pBlueG/SA-MP-MySQL/releases/tag/R41-4) |
| BCrypt for SAMP | 2.2.3 | [https://github.com/lassir/bcrypt-samp/releases/tag/v2.2.3](https://github.com/lassir/bcrypt-samp/releases/tag/v2.2.3) |
| ZCMD | 1.0. | [https://github.com/Southclaws/zcmd/blob/master/zcmd.inc](https://github.com/Southclaws/zcmd/blob/master/zcmd.inc) |
| easyDialog | 2.0 | [https://github.com/Awsomedude/easyDialog/releases](https://github.com/Awsomedude/easyDialog/releases) |
| Sscanf2 | 2.8.3 | [https://github.com/maddinat0r/sscanf/releases/tag/v2.8.3](https://github.com/maddinat0r/sscanf/releases/tag/v2.8.3) | 
