# steam-epic-launcher
Use Steam to launch Epic Games Launcher games

# What is this?
All credit goes to SeanZWrites:

https://seanzwrites.com/posts/how-to-play-epic-games-on-steam-and-steamlink

This is a shameless lift of the C# code at the end of that post.

### Build

```
# Create the build artifacts
dotnet build

# Build for Windows ('win-x64')
TARGETRUNTIME=win-x64
dotnet publish --output ./bin --runtime win-x64 --configuration Release -p:PublishSingleFile=true -p:PublishTrimmed=true --self-contained true
```

### Steam: "Add Non-Steam Game"

Use the "\[directory\]\bin\SteamLauncher.exe"