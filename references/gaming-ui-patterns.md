# Gaming Web App UI Patterns

## Server controls

### Start
Button: **Start server**

Pending state: **Starting**

Success: **Server started**

Failure:
- **Server failed to start. Check the console for the latest error.**

Do not say **Server online** until the system actually knows the server is ready for players.

### Restart
Button: **Restart server**

If restart causes player disconnects, surface that consequence when confirmation is useful:
- **Restart server?**
- Connected players will be disconnected.
- [Cancel] [Restart server]

Do not require confirmation for routine restart if the product intentionally optimizes for fast admin control and the consequence is already well understood.

### Stop
For active multiplayer servers, consider consequence:
- **Stop server?**
- Connected players will be disconnected.
- [Cancel] [Stop server]

## Reinstall and wipe

### Reinstall
Explain file/data impact precisely.

- **Reinstall server?**
- Server software will be reinstalled. Custom files may be replaced. Back up anything you want to keep.
- [Cancel] [Reinstall server]

Only mention deletion if the product actually deletes data.

### Wipe
- **Wipe server data?**
- This removes the current world and player data. Server settings are kept.
- [Cancel] [Wipe server data]

If settings are also removed, say so.

## Backup and restore

### Backup
Button: **Create backup**
State: **Backing up**
Success: **Backup created**

Failure:
- **Backup failed. There isn't enough storage available. Free up space and try again.**
- **Backup failed. Try again or check the activity log for details.**

### Restore
- **Restore this backup?**
- Current server data will be replaced with the selected backup.
- [Cancel] [Restore backup]

If the platform automatically creates a safety backup first, state that.

## Status cards

A useful server status card may include:
- Running state
- Player count
- Current map
- Uptime
- Public address
- Version
- Update status

Use labels, not prose, for dense operational surfaces.

Example:
- Status: Running
- Players: 42 / 80
- Map: Narva
- Uptime: 6h 18m

## Empty states

### No servers
**No servers yet**
Create your first server to get started.
[Create server]

### No backups
**No backups yet**
Create a backup before making major changes.
[Create backup]

### No players
**No players online**
Players will appear here when they join the server.

### No search results
**No matching servers**
Clear your filters or try a different search.

## Errors

### Unknown failure
When the cause is unknown:
- **Server failed to start. Check the console for details.**

Do not invent:
- Network issue
- Configuration error
- DDoS attack

unless the system has evidence.

### Permission failure
- **You don't have permission to restart this server.**
- Ask an administrator for access.

### Connectivity
- **Connection lost**
- Reconnect to continue viewing live console output.
- [Reconnect]

### Rate limit
- **Too many requests**
- Wait a moment and try again.

If a precise retry time is known, show it.

## Updates

### Update available
- **Update available**
- Version 1.2.3 is ready to install.
- [Update server]

### Update in progress
- **Updating**
- Server controls are temporarily unavailable.

### Update complete
- **Update complete**
- Server is ready to start.

Do not say **ready to play** unless readiness checks support that claim.

## Maintenance

### Planned maintenance
- **Scheduled maintenance**
- Server controls will be unavailable from 02:00–03:00 UTC. Running servers are not affected.

Only include exact times when known.

### Active maintenance
- **Maintenance in progress**
- Server controls are temporarily unavailable. Running servers are not affected.

### Incident
- **Server controls are currently unavailable**
- We're investigating. Running servers are not affected.

Avoid apologies as the primary information.

## Billing

### Payment failed
- **Payment failed**
- Update your payment method to keep the service active.
- [Update payment method]

### Expired
- **Subscription expired**
- Renew to restore server access.
- [Renew subscription]

### Suspended
- **Service suspended**
- The server is offline and controls are unavailable. Renew or contact support.

Only describe data retention if the actual retention policy is known.

## Community

### Discord
- **Join the community**
- Get server updates, support, and announcements on Discord.
- [Join Discord]

### Whitelist
- **Whitelist active**
- Only approved players can join this server.

### Ban
Admin view:
- **Banned for 7 days**
- Reason: Teamkilling
- Ends: 14 Oct 2026

Player view should expose only information intended for the player.

## Toasts

Keep routine toasts short:
- Changes saved
- Server started
- Server stopped
- Restart requested
- Backup created
- IP address copied

Do not add celebration unless the action deserves it.

## Notifications

Use notification copy only for information that remains useful outside the current screen.

Good:
- Server update completed
- Backup failed
- Payment failed
- Scheduled maintenance starts in 30 minutes

Avoid notifying for trivial actions the user just performed and already sees confirmed.
