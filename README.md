# steam-epic-launcher
Use Steam to launch Epic Games Launcher games

# What is this?
All credit goes to SeanZWrites:

https://seanzwrites.com/posts/how-to-play-epic-games-on-steam-and-steamlink

This is a shameless lift of the C# code at the end of that post.

### Build

I built this on Ubuntu.

```
# Create the build artifacts
dotnet build

# Build for Windows ('win-x64')
TARGETRUNTIME=win-x64
dotnet publish --output ./bin --runtime $TARGETRUNTIME --configuration Release -p:PublishSingleFile=true -p:PublishTrimmed=true --self-contained true
```

### Steam: "Add Non-Steam Game"

Use the "bin\SteamLauncher.exe" executable.