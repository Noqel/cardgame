# Absolutely Worthless

A dependency-free, server-authoritative multiplayer auction prototype for 2–6 players. Requires Node.js 22 or newer.

```sh
npm start
npm test
```

Open the app on port 3000. Create a table and share its code with friends connected to the same server. Separate browser tabs have separate player sessions. Eight lots, six secret goal types, sixteen objects, private inspections, public bluff claims, bundling, and automatic final scoring are implemented. Rules are shown in the lobby. Set `PORT` to change the listening port.

The browser client polls the server every second. State stays in memory; restarting loses games. Keep your tab to reconnect with its session token. Players cannot yet be removed and there is no turn timeout, so a disconnected player can stall a game. This is a prototype, not a production or Steam release: Steamworks authentication, lobby invites, packaging, persistence, abuse controls, and deployment are future work. No Steam credentials are required to develop the current version.
