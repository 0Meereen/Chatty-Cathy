# Update-Chatty-Cathy Change-Log
<h1 align="center">
  <br>
  <img src="https://cdn.discordapp.com/attachments/1054749393238097962/1060231996535750656/20221230_152013_0000-removebg-preview.png" alt="Chatty Cathy Discord bot">
  <br>
  Chatty Cathy Discord bot
  <br>
</h1>

### 📝 ToDo 

- [ ] lyrics command
- [ ] secret 

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


