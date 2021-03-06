# Private Dedicated Gaming Servers | Linux Edition

**Let's get started with installing a server on linux.**
You will need to have root access for flawless installation.

##### Once logged in start with these commands, This will open your ports.
 > sudo ufw allow 28960/tcp
 > 
 > sudo ufw allow 28960/udp
 > 
 > sudo ufw disable
 > 
 > sudo ufw enable
 > 

###### Let's upgrade all packages and update them.
 > apt-get update && apt-get upgrade
 
 ##### Let's install an OS for our images just in case called.
  > apt-get install screen
  
 ##### Now let's switch our architecture to a game readable one.
 > dpkg --add-architecture i386
 > apt-get update

##### Create a folder where the game will be stored.
 > cd ~
 > mkdir {NAME OF GAME FOLDER}
 
 ##### Go inside the folder you just created and download needed files. (Skip past line 20-30 if you are adding the files manually.)
 > cd {NAME OF GAME FOLDER}
 > wget {ADD LINKS}
 
 ##### If you need to extract a tar file use this command. 
 > tar -xvjf {FILE NAME}
 
 ##### If you are unzipping the file then use this command.
  > unzip {FILE NAME}
 
 Make sure you have the game installed on your computer, Files must be up to date or else you will get connection issues.
 
 ##### You will now need to make the file executable inside your server.
  > chmod +x {GAME APPLICATION (No extension, *sh, *so, etc)
  
 At this point you will need to create a **server.cfg** file if you haven't yet. This is the file that configures your game as you desire, Once this part is down see below to run your server.
 
##### This is execute inside your server console.
 > ./{APPLICATION} +exec "server.cfg" +set fs_game "mods/ExampleMod" +map_rotate +set dedicated 2 +set net_ip 192.168.1.1

---

> 
> #### Github By Sin
>

*We aren't just going to baby feed you so you will need to learn somehow.*
