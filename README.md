# Update-Chatty-Cathy Change-Log
<h1 align="center">
  <br>
  <img src="https://cdn.discordapp.com/attachments/1054749393238097962/1060231996535750656/20221230_152013_0000-removebg-preview.png" alt="Chatty Cathy Discord bot">
  <br>
  Chatty Cathy is a Discord bot designed to help you manage your server and play music! The bot comes equipped with several features, including XP system, level tracking, and a music player.
  <br>
</h1>

Support : https://discord.gg/A7gcRnECGU
Vote : https://top.gg/bot/1045262853508186152

-------------------------------------------------------

═════════════════════════════════
              Patch Notes - Version 1.8.0
═════════════════════════════════

New Features:
- Added support for SoundCloud to search and play music from SoundCloud.
- Music search has been adjusted to be more accurate and efficient.
- Added a confirmation for removing user data.
- An integration message is now displayed when the playlist is done.
- The playing embed is now automatically updated when the playing music is changed.

Bug Fixes:
- Fixed a bug that caused the bot to leave the voice channel during music playback.
- Fixed a bug that caused errors with the volume command for multiple guilds.

Other Changes:
- The "more" button event is now removed after 15 seconds for a better user experience.
-Modified the typography of the playing music title to make it easier to differentiate from other text.



Patch Notes - Version 1.7.0:

- [X] Fixed issue with the volume command not working properly.
- [X] Corrected a typo in the clear command that was causing errors.
- [X] Fixed a bug where XP was being calculated incorrectly.
- [X] Renamed the dashboard command to rank for improved clarity.
- [X] Added a new feature: filter. Users can now filter search results more easily.
- [X] Added a new command: disablefilters. This command allows users to - [X] disable filters.
- [X] Added the ability to earn XP randomly between 10 to 200.
- [X] Added cooldowns for all XP-earning commands to prevent spamming.
- [X] Disabled the "back" button if there is no previous track.
- [X] Added a new premium button (coming soon).
- [X] Ater loading track, message delete
- [X] Ater loading playlist, message delete
- [X] Fix error typo

Update 1.6.3

- [X] Ater loading track, message delete
- [X] Ater loading playlist, message delete
- [X] Fix error typo

Update 1.6.2

- [X] Change command "xp" to "level"
- [X] Delete rank command
- [X] Add button shuffle
- [X] Fix clear button

Update 1.6.1


- [X] Fix crash when you using command in DM.
- [X] Fix Typo 
- [X] Update discord-player 6.1.1

Update 16.1.0

- [X] Xp system multi guild.
- [X] Disable button back ( he dont work )
- [X] New embed for dashboard, rank.
- [X] Add system status (only for Chatty Team).
- [X] Addxp disable (Rework soon).
- [X] Remove old code.
- [X] Earn xp work for the command core now.

Update 1.6.0
- [X] Rework help command
- [X] System earn xp (Test)
- [X] Command dashboard
- [X] Increase perf
- [X] Finally back button work.
- [X] Fix crash with voice channel temporary
- [X] New command :
 - xp
 - register
 - unregister
 - addxp
 - addlevel
 
 ```js
      const xpStatusMessage = `🎓 Here is your XP status:
- Level: **${userData.level}**
- Current XP: **${userData.xp}**
- XP to next level: **${nextLevelXp - userData.xp}**
- Total XP: **${userData.xp + (userData.level - 1) * nextLevelXp}**`;
```
 
 
 -----------------------------------------------------

Update 1.5.0

- Fix back command.
- Massive typo change.
- Compatible discord-player V6.
- Queue destroy sometimes for nothing fixed.
- Add New button "more" ( New controller available). 
- Add save music command ( pm link music when u use button).
- Increase performance. (the hosting is much more efficient)
- New typo in trackAdd.

Update 1.1.0

- Cleaning of the writing
- Add embed ( duration, progressbar, external url)
- thumbnail spotify / youtube
- fluidity increase



Update 1.0.0

- Fix Music crash after 40-50 seconds.
- Error : bot stops playing after a minute in the song.
- Temporary fix:
- Edit the file located at /node_modules/@discordjs/voice/dist/index.js on line 1429

```js
  addStatePacket(packet) {
    this.configureNetworking();
    this.packets.state = packet;
    if (typeof packet.self_deaf !== "undefined")
      this.joinConfig.selfDeaf = packet.self_deaf;
    if (typeof packet.selfmute !== "undefined") 
      this.joinConfig.seldMute = packet.self_mute;
    if (packet.channel_id) 
      this.joinConfig.channelId = packet.channel_id;
  }
};
```

Update 1.0
- Fix error in console
- shuffle command add
- playnext command add
- Fix typo

Update 0.9B (2)
- Fix crash "pause"

Update 0.9B
- Emoji support
- Change typo "Events start"
- Fix command "queue"
- Remove all command <Private message>
- Fix crash (queue so long)
- Fix permission erreur
- Add command "/version"
- Change typo "ping"



Update 0.6B

- Add button "Stop"
- Remove wrong text.
- Change icon profile.
- Fix little bug minor.
- Fix support 24/7.
- Fix Support spotify.

```js
playlist.tracks = spotifyPlaylist.trackList.map((m) => {
    const data = new Track_1.default(this, {
        title: m.title ?? "",
        description: m.description ?? "",
        author: m.subtitle ?? "Unknown Artist",
        url: m.external_urls?.spotify ?? query,
        thumbnail: m.album?.images?.[0]?.url ?? "https://www.scdn.co/i/_global/twitter_card-default.jpg",
        duration: Util_1.Util.buildTimeCode(Util_1.Util.parseMS(m.duration)),
        views: 0,
        requestedBy: options.requestedBy,
        playlist,
        source: "spotify"
    });
    return data;
};
```


