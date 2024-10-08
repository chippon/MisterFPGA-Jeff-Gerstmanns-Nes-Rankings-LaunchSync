# Jeff Gerstmanns Nes Rankings LaunchSync for MiSTerFPGA
LaunchSync File for the MisterFpga of Jeff's Nes Rankings.

# LaunchSync Info
* LaunchSync is part of https://github.com/wizzomafizzo/mrext MiSTer Extensions project.

* More info at https://github.com/wizzomafizzo/mrext/blob/main/docs/launchsync.md
  
# Thanks https://8bitnintendo.science/
* This is generated off the https://8bitnintendo.science/ github's "list.csv" and then converted to a LaunchSync .sync file.

# What does this do?
Creates a Main Menu folder Named "The Science - Jeff Gerstmann's Nes Ranking"
![alt text](https://github.com/chippon/Jeff-Gerstmanns-Nes-Rankings-LaunchSync/blob/df484dab997dd21d8122dfbd84b08a745ddeed51/data/Main_Menu_Science.gif)

 
Inside that folder the games (that were found at sync) can be played
![alt text](https://github.com/chippon/Jeff-Gerstmanns-Nes-Rankings-LaunchSync/raw/main/data/Game_List.png?raw=true)

* The [NOT FOUND] games will still load into the emulator so you don't have to menu out.
  
# How To
* 1- Download the Jeff_Nes_Ranking.sync file and place it in your /media/fat/ folder on your MisterFpga.
* 2- At the Main Mister Menu -> scripts -> run launchsync
* 3- The script should find the new sync file and search your games looking for matches.

# Issues I ran into
Timeout during build of games db at startup of LaunchSync
* I turned off CIFS to unmount my networked games. Then loaded a nes set onto my main flash cart.
* After I turned CIFS back on and mounted my drives. The games were still accessible. (hard coded to the flashcard after generation)
   
Games with [NOT FOUND] in the name
* Tested on a everdrive set, the sync was unable to find 70 off the 375+ games. Your Milage may vary.
* You can edit or add more matches for the games that were not found in the sync file.




# Updates?
* on the backend, hoping to use more general regex in the build script to get better matches from the list.csv.
* fix list that matches the list.csv and replaces phrases then see if it can get more matches. (mario bros. = mario bros. + duck hunt) etc.
* This was made with bash, the script can be found in the data folder as Build_Sync_List.sh

# <>
  
