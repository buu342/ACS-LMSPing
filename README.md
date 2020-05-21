# LMSPing
A player position tracker for Zandronum, created to prevent camping in LMS games. It allows players to, after a cooldown, press a button to reveal/track other players' positions. Works on other gamemodes as well. In Team games, pings show team colors as well.<br/><br/>
Pinging relies on serverside values, and I don't reveal any information to clients which they don't already know about, so it should be safe to use.<br/><br/>
This WAD requested by Marcaek.
<br/><br/>
### Serverside configuration
```c
lmsping_pingonspawn = false; // Can someone ping as soon as they spawn?
lmsping_cooldown    = 30;    // Cooldown between uses in seconds (0 for not using time based cooldown)
lmsping_duration    = 5;     // 0 to only show last location, any other value to hold it for those many seconds
lmsping_coolonfrags = 0;     // Reset cooldown on X many kills
```
<br/>

### Clientside configuration
```c
cl_lmsping_usesounds    = true; // Use radar sounds
cl_lmsping_showcooldown = true; // Show the cooldown above the statusbar
```
<br/>

### How to use
  **1)** Include this WAD in your server's wad list.<br/>
  **2)** That's pretty much it...
<br/><br/>
### Changelog
**Version 1.0**
* Initial release
