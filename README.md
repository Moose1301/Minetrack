<p align="center">
	<img width="120" height="120" src="assets/images/logo.svg">
</p>

# Minetrack
Minetrack makes it easy to keep an eye on your favorite Minecraft servers. Simple and hackable, Minetrack easily runs on any hardware. Use it for monitoring, analytics, or just for fun. [Check it out](https://minetrack.me).

This instance is public at: [track.antiskid.club](https://track.antiskid.club)

### Features
- 🚀 Real time Minecraft server player count tracking with customizable update speed.
- 📝 Historical player count logging with 24 hour peak and player count record tracking.
- 📈 Historical graph with customizable time frame.
- 📦 Out of the box included dashboard with various customizable sorting and viewing options.
- 📱(Decent) mobile support.
- 🕹 Supports both Minecraft Java Edition and Minecraft Bedrock Edition.
- 
## Docker
Minetrack can be built and run with Docker from this repository in several ways:

### Build and deploy directly with Docker
```
# build image with name minetrack and tag latest
docker build . --tag minetrack:latest

# start container, delete on exit
# publish container port 8080 on host port 80
docker run -e MINETRACK_PORT=8081 -e MINETRACK_DATA=/opt/tracker --rm --publish 80:8080 minetrack:latest
```
