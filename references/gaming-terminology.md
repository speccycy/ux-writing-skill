# Gaming Web App Terminology

Use consistent terms across the product. Do not swap synonyms for variety.

## Core hosting terms

### Server
A game server the customer operates or joins.

Use:
- Start server
- Server status
- Server offline

Do not use **instance** unless the product explicitly exposes an instance concept.

### Instance
A managed application or service unit distinct from the user's game server.

Use only when product architecture requires this distinction.

### Node
The host machine or infrastructure location that runs one or more servers.

Use when users need to understand infrastructure placement, capacity, or migration.

### Location / Region
Use **Location** for a physical hosting location such as Singapore or Bangkok.
Use **Region** only if the platform groups locations into a larger regional abstraction.

### Slot
A player-capacity unit when the game or hosting plan is sold by player slots.

Avoid using **seat** for game-server capacity.

## Server lifecycle

### Start
Launch a stopped server.

### Stop
Shut down the server process.

### Restart
Stop and start the same server.

### Reinstall
Rebuild or reinstall server software. This may remove or replace files depending on product behavior.

Never use **reinstall** as a synonym for restart.

### Reset
Return a setting or configuration to a known default.

### Wipe
Remove game/world/player progression data when that is the established game-server action.

Always state what data is removed and what is kept.

## Data and recovery

### Backup
A saved copy intended for recovery.

### Restore
Replace current data with data from a selected backup.

### Snapshot
Use only if the underlying product actually creates snapshots distinct from backups.

### World / Save data / Player data
Use the term the game or product exposes. Do not merge these concepts if they have different retention behavior.

## Access and management

### Console
Live output and command interface.

### RCON
Remote console protocol or connection. Keep as RCON for technical audiences.

### Query port
Port used for server discovery/status queries.

### Game port
Port used by players or the game protocol.

### Whitelist
Use when the game/community convention is well established. If the product uses an alternative term such as **Allowlist**, keep terminology consistent with the product.

### Reserved slot
A player slot held for eligible users.

### Queue
Waiting list before joining a full or restricted server.

## Add-ons

### Mod
A game modification.

### Plugin
An extension loaded by a server framework, panel, or supported plugin system.

### Workshop item
Use when referring specifically to Steam Workshop content.

Do not collapse Mod, Plugin, and Workshop item into one term unless the product itself does.

## Reliability and security

### DDoS protection
Use for protection against distributed denial-of-service attacks.

Do not use **anti-DDoS** and **DDoS protection** interchangeably across the same product unless required by vendor terminology.

### Mitigation
Use when describing an active filtering/protection event.

### Maintenance
Planned or operational work affecting a product or feature.

### Incident
Unplanned degradation or outage.

### Degraded
Available but operating below normal quality or capacity.

### Unavailable
Not usable.

## Billing

Keep these states distinct:
- Active
- Payment pending
- Payment failed
- Renewal scheduled
- Expired
- Canceled
- Suspended
- Terminated
- Refund requested
- Refund processed

Never use **expired**, **canceled**, **suspended**, and **terminated** as synonyms.

## Status labels

Prefer exact process states:
- Starting
- Running
- Stopping
- Restarting
- Updating
- Backing up
- Restoring
- Offline
- Maintenance
- Degraded
- Unavailable

Avoid **Online** if the server process is not yet ready for players.
