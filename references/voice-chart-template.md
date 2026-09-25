# Voice Chart Template for Gaming Web Apps

Use this template to define a consistent voice for game-server hosting panels, dashboards, community tools, and gaming SaaS products.

A useful voice chart has:
- a small set of durable voice concepts
- concrete characteristics
- examples of what to do
- examples of what to avoid

Do not turn the chart into a list of marketing adjectives. Each concept must change how UI copy is written.

## Recommended baseline

### Concept 1: Clear and direct

**Voice characteristics**: Scannable, specific, plain language

**Description**: Put the state, action, or consequence first. Use the shortest wording that still lets users act correctly.

**Do**:
- Server failed to start. Check the console for details.
- Restart server
- Backup created

**Don't**:
- An error occurred while attempting to perform the requested operation.
- Proceed with server restart operation
- Your backup has been successfully created for you

---

### Concept 2: Confident and calm

**Voice characteristics**: Reliable, composed, operational

**Description**: Keep failures and incidents factual. Do not exaggerate, panic, or bury useful information in apologies.

**Do**:
- Server controls are temporarily unavailable.
- Connection lost. Reconnect to continue.

**Don't**:
- Critical system failure!
- We sincerely apologize for any inconvenience this unfortunate issue may have caused.

---

### Concept 3: Helpful

**Voice characteristics**: Actionable, supportive, clear

**Description**: When a user can recover, explain the next useful action. When the system does not know the cause, do not invent one.

**Do**:
- Backup failed. There isn't enough storage available. Free up space and try again.
- No matching servers. Clear your filters or try a different search.

**Don't**:
- Backup failed.
- No results.
- Network error. (unless the system actually knows this)

---

### Concept 4: Technical when needed

**Voice characteristics**: Accurate, specific, domain-aware

**Description**: Preserve technical terms when they help users operate or troubleshoot the product. Explain only when the audience needs it.

**Do**:
- RCON connection failed.
- Query port is already in use.
- DDoS mitigation is active.

**Don't**:
- Technical issue detected.
- Something is wrong with networking.
- Simplify every domain term into vague consumer language.

---

### Concept 5: Gaming-friendly

**Voice characteristics**: Modern, approachable, restrained

**Description**: Sound at home in a gaming product without forcing slang, memes, or competitive language into routine operations.

**Do**:
- Ready to play
- Join the community
- Invite your squad

**Don't**:
- GG EZ, server deployed!
- Epic gamer server unlocked!
- Bro, your server died.

## Tone adaptations

The product voice stays consistent, but tone changes with context.

### Routine controls
Fast, neutral, efficient.

Examples:
- Start server
- Restarting
- Changes saved

### Errors
Calm, factual, recovery-focused.

Example:
- Server stopped unexpectedly. Check the console for details.

### Destructive actions
Serious and explicit.

Example:
- Wipe server data?
- This removes the current world and player data. Server settings are kept.

### Billing
Precise and neutral.

Example:
- Payment failed. Update your payment method to keep the service active.

### Community
Friendly and inviting.

Example:
- Join the community on Discord.

### Moderation
Neutral and factual.

Example:
- Banned for 7 days. Ends 14 Oct 2026.

## Product-specific customization

Adapt this baseline to the product instead of replacing it with unrelated personality traits.

Useful questions:
1. Which users are primary: players, server owners, community admins, hosting customers, or technical operators?
2. How technical is the interface?
3. Which actions can cause downtime or data loss?
4. Does the brand want more energy in community/marketing surfaces than in operational controls?
5. Which terms are canonical across the product?

For bilingual products, define voice once at the intent level, then localize English and Thai independently. Do not require Thai to mirror English wording.
