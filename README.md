# Bombsquad modder server files (bcs modified)

Special Thanks to sara and PcModder..!

Basic knowledge of Linux
A VPS (e.g. Amazon Web Services, Microsoft Azure)
Any Linux distribution.
It is recommended to use Ubuntu.
Python 3.10
1 GB free Memory (Recommended 2 GB)

Getting Started

This assumes you are on Ubuntu or an Ubuntu based distribution.

Download server files.
git clone <github-link>

## well short way to download all required modules in one go :
1. chmod 777 bs_requirement.sh
2. sudo ./bs_requirement.sh

it will download all required packages.
Now you can edit rest files

## Update and install software-properties-common:

sudo apt update; sudo apt install software-properties-common -y

## Add python Deadsnakes PPA:
sudo add-apt-repository ppa:deadsnakes/ppa

## Install Python 3.10:
sudo apt install python3-pip python3.10-dev python3.10-venv

## Create a tmux session.
tmux new -s 43210

cd Bombsquad-Ballistica-Modded-Server

Now edit config.yaml in root dir change server name, port, admins, playlist, team name etc.. Making the server files executable.

chmod 777 bombsquad_server
chmod 777 dist/bombsquad_headless
Starting the server

sudo ./bombsquad_server
If ports are open, you can connect to your server now.

More Configuration
Open dist/ba_root/mods/setting.json in your prefered editor and change values according to you.

This assumes that you already used bcs files, and you know how to edit server files like adding owner and other stuff.

# Features
well this script inclues all bcs Features and more advanced features which are added by me.
To know bcs features visit https://github.com/imayushsaini/Bombsquad-Ballistica-Modded-Server

### The game cmds which we added : 
zoommessage (zm),
fall,
speedon,
hug,
icy,
spaz,
top,
setscore,
zombieall,
boxall,
texall,
kickall,
ooh,
spazall,
acl (admin cmd list) ,
vcl ( vip cmd list ) ,
tint,
ac,
comp ( to file complaint agaist player, but u need to setup dc bot to use this cmd),
rainbow,
Playsound,

 * Time and member count in textonmap 
 * Modified season reset count down which is fully visible

# Coinsystem:

1.Added a coins/tickets system and shop. Players can buy effects and tags with tickets. You can modify the expiry time of purchases. There's also a command to remove paid effects (/rpe 113) so players can correct their purchases.

2.Introducing Daily Claim:
Well, you can turn off questions and use the daily claim feature, so people can't use the auto-answer plugin, engaging players more to play daily.

# Discord Bot:

## Cool Modified Stats UI
### ![image](https://github.com/hypervortex/Bombsuqad-Modded-Server-Files/assets/75498823/250b1511-627d-44ab-b397-98077c27246b)

* You can easily add admin, VIP, owner, custom tags, effects, staff, and mods directly from your Discord server.
* Efficient Server Management using Discord commands. You can do everything from Discord, like adding effects, muting, tags, roles, restarting server, getting player info such as rank, * * * score, device id, IP, and many more data. To get more details, set up the bot and try v!help.
* Advanced banning system using MongoDB. If you are hosting multiple servers, then it's a very useful feature for you. Just ban once, and it will get banned in all servers, and even if you * lose server files data, your banlist is still safe.
* Added a complaint feature from the game to Discord, so people don't need to leave the game to complain on Discord.
* Added Notify feature. If you used BCS manager, then you may know about the feature regarding subscribed players. You get notified when that subscribed player joins the server, so this is * the same feature but notifies in the Discord server. You just need to add another channel id and role to ping, so you will get notified.
* Player Data Check: Easily check player ranks and see the top 10 players on your servers.
* Bot security: Added security to ensure only authorized members and servers can execute commands.
* Enhanced Custom Effects: Modified existing effects such as fairydust and sweat and added more beardmods(1.8) effects.
* Added autoadmin along with the score. So rank 1, 2, 3 with specified score will get admin and VIPs.
* Check setting json for more settings. You can set up your bot prefix as you want.
