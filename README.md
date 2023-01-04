# Update-Chatty-Cathy Change-Log
<h1 align="center">
  <br>
  <img src="https://o.remove.bg/downloads/e179117d-3ab3-4c5f-a031-66b84c677a6e/chatty_cathy-removebg-preview.png" alt="Chatty Cathy Discord bot">
  <br>
  Chatty Cathy Discord bot
  <br>
</h1>

### 📝 ToDo 

- [ ] lyrics command
- [ ] secret 

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


