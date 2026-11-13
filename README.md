# BRAY — Online Multiplayer Card Game

Real-time 2–6 player card game using Node.js, Express and Socket.IO.

## Run locally
```bash
npm install
npm start
```
Open http://localhost:3000 in multiple browsers. Create a room and share its six-character code.

## Deploy on Render
1. Push this repository to GitHub.
2. Create a Render Web Service connected to this repository.
3. Build command: `npm install`
4. Start command: `npm start`
5. Health check: `/health`

## Prototype rules
- 2–6 players, 7 cards each.
- Match active colour or top card value/action.
- Skip, Reverse, Draw 2, Wild and Wild +4.
- Players are ranked as they empty their hand; final remaining player ranks last.

## Limitations
This MVP stores rooms in server memory. Server restarts clear active games. Add persistent storage, reconnect tokens, rate limiting and automated tests before production use.
