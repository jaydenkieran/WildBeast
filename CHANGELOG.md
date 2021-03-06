# 3.0.0
## Release phase
### 3.2.0
Internal tweaks.   
Retired XL formatting in help for INI formatting.   
WildBeast now alerts the user with a more descriptive error message if the config file is invalid or missing.   
The special word `%user` now resolves to a mention instead of the username.   
`INVALID` doesn't get dumped to the playlist anymore if YouTube videos from a YT playlist fail to fetch, they'll get silently dropped instead.   
`leave` is renamed to `leave-server` to avoid confusion.    

### 3.1.1
Fixed welcome message not sending properly when set to private.   

### 3.1.0
Welcome messages can now be send via private messages.   

### 3.0.0
Masters are now at `Infinity` instead of 9.   
Voice channel join messages now use a customized prefix if available.    

## Beta phase
### 3.0.0-beta.6
Introduced `shuffle` and `voteskip` as music commands.    
Introduced `master` as a new access level.    
Several small tweaks and improvements.    
 
### 3.0.0-beta.5
Several improvements.    

### 3.0.0-beta.4
Added the ability to set roles to access levels.

### 3.0.0-beta.3
Improved performance from YouTube playlist fetching.     
Added `shardmode`    

### 3.0.0-beta.2
Fixed initial setup misbehaving if user was sure about using a normal Discord account.    
Enabled versionchecker.   
Fixed `voice` not working properly if user was not connected to any voice channel.    
Fixed some internal quirks.    

### 3.0.0-beta.1
Introduced tags.   

## Alpha phase
### 3.0.0-alpha.2
Enabled command alias system.   
Changed giphy endpoint for more randomness.   
Added a `noDM` key.   

### 3.0.0-alpha.1
Initial release, featuring all-new code.

# 2.0.0
## Release phase
### 2.1.1
Added timeouts.    
Changed `request` to only accept full links from now on.    
Made preparations for a future update.     

### 2.1.0
Changed callbacks to promises.     
Removed `playliststart`, playlists start automatically after the first video has been entered.     
Extended timeout for initial join.     
Several small tweaks.     

### 2.0.0
Revamped database system.
Added token login support for the upcoming official Discord API.         
Added expansive server-specific customization options.     
Added user tracking for namechanges.      
Added an upgrade script for users to upgrade from gamma.7 to 2.0.0     
Removed server defaulting system.     
Removed unneeded and unfinished files in `runtime`.      
Removed unnecessary fluff from `config.json`.      
Removed `welcoming-whitellist.json`, this is now handled by `customize`.     
Removed `birds`, `ìdle` and `online`, `idle` and `online` are replaced with `setstatus`.     
Temporary removed server blacklisting system, this will be reintroduced later.      

## Gamma phase
(Gamma is a real thing in software development by the way, it's a synonym for RC (Release Candidate))
### 2.0.0-gamma.7
Changed welcoming system to adhere to a whitelist instead of being global.    
Added server blacklisting for `join-server`.    
**IMPORTANT** Changed `join-server` to use mentions instead of usernames, the new invocation is `join-server @WildBeast <instant-invite>`, change `WildBeast` with your bots username.

### 2.0.0-gamma.6
Added YouTube playlist support.    

### 2.0.0-gamma.5
Removed `play` and `yt-play`.    
Added playlisting for YouTube video's.    

### 2.0.0-gamma.4
Revamped music streaming permissions due to the way the normal permissions handle.    
Added some extra commands.    
Hopefully improved the reliability of `stop` for music streaming.   
Made preparations for a future update.    

### 2.0.0-gamma.3
*This is a relative small update.*   
Added YouTube streaming.   

### 2.0.0-gamma.2
Added some extra commands.   
Revamped debug mode and verbose logging.   
Changed `setowner` to set server owner to level 4 instead of level 3.  
Changed commands that where at level 4 to level 5.    

### 2.0.0-gamma.1
Added a timeout feature.    
**GET HYPED FOR MUSIC STREAMING!**      
Changed `versionchecker.js` ability to check for beta versions to gamma version checking.    
Moved to LevelDB instead of Redis for handling permission storage and handling timeouts.      

## Beta phase
### 2.0.0-beta.5
Fixes several problems caused by 2.0.0-beta.4   
Added an *incomplete* server defaulting system.   
Added `setstatus`.     
Changed the fixed length of `cmd_prefix` to a dynamic length.   
Changed the fixed character prefix to switch to mention activation if desired.   

### 2.0.0-beta.4
Fixed `myapifilms_token` not existing.  
Fixed problems with `++setowner`.  
Added `debug_mode` and `verbose_logging`. *(Note, only enable these on request of the devs!)*   
Added a config value that'll change the way `++help` functions.  
Updated the layout of `config.json`, **meaning that users need to remake their config files.**

### 2.0.0-beta.3
Fixed `giphy.js` not having requires.  
Fixed `suffix` not behaving accordingly.    
Added `++fortunecow`, `++randomcat`, `++rule34` and `++leetspeak`.   
Added `mashape_key` to `config.json`.   
Removed NSFW flags from commands that did not need them, as this will cause problems with `++help`.  
Removed `deletion.js`, as this is needlessly split.   

### 2.0.0-beta.2
Updated `versionchecker.js` to check for beta updates.   
Moved to double prefix activation instead of single prefix activation as requested by Discord API, we recommend using `++`.   
Bot is also compliant with the [Discord bot best practises](https://github.com/meew0/discord-bot-best-practices), also requested by Discord API.    

### 2.0.0-beta.1
Initial release of DougBot 2.0, featuring new permission system and stability improvements.

## Alpha phase
Nothing too interesting lol.
