# Bikar Server

A Mac app that helps run the network behind [Bikar](https://www.bikar.app), the free and open-source online
training app. Bikar has no company servers: riders' phones find each other and race directly. Bikar Server is a
helper that anyone can run on a spare Mac.

**How the network works: [bikar.app/network](https://www.bikar.app/network)** ·
**The app: [tomfry/bikar](https://github.com/tomfry/bikar)**

> The code isn't here yet. Bikar Server grows out of Bikar Monitor, the network window in the main project, and
> will arrive with a permissive licence alongside the app's code. Watch this repository to hear when it lands.

## What it does

- **Helps riders connect.** It joins the network as a bootstrap and relay node. Riders on mobile data or behind
  strict routers often can't reach each other directly, so it passes their packets on. Every packet is signed by its
  sender, so a relay can't change what it carries.
- **Shows who's on the network.** Which maps have riders on them, live races with their standings, and the health
  of the links and of the DHT lookups.
- **Fills quiet roads, if you want it to.** It can add computer racers to the worlds, so a rider who turns up at
  a quiet hour still has someone to race. They're marked as bots in every result.

## What it doesn't do

- It holds no accounts and stores no riders' rides. The network doesn't depend on it: riders find each other through
  the Mainline DHT and their own Wi-Fi whether or not any Bikar Server is running.
- It never runs anything a peer sends it.

## Links

- [Bikar, the app](https://github.com/tomfry/bikar)
- [How the network works](https://www.bikar.app/network)
- [Open source and how to help](https://www.bikar.app/open-source)
- [Support](https://www.bikar.app/support) · support@bikar.app
