---
name: gaming-webapp-ux-writing
description: Write and review UX copy for gaming web apps, game-server hosting panels, dashboards, control panels, billing flows, community tools, and technical product interfaces in English and Thai. Use for buttons, labels, forms, server states, destructive actions, errors, warnings, notifications, onboarding, empty states, maintenance messaging, subscriptions, player/community features, localization, terminology audits, and product voice. Optimize for clear, concise, confident, helpful copy that stays technically accurate without sounding robotic, corporate, or overly gamer-styled.
---

# Gaming Web App UX Writing

Write interface copy for gaming products and game-server platforms. Keep the original UX-writing priorities: purposeful, concise, conversational, and clear. Add two domain requirements: **operational accuracy** and **state awareness**.

## Core standards

Every UI string must be:

1. **Purposeful** — Help the user understand, decide, recover, or act.
2. **Concise** — Remove words that do not change meaning or action.
3. **Natural** — Sound like a real product, not generated or translated copy.
4. **Clear** — Prefer specific actions and states over vague wording.
5. **Technically accurate** — Do not simplify a server or billing state until it becomes misleading.
6. **State-aware** — Reflect whether an action is pending, running, failed, unavailable, destructive, or complete.

## Product voice

Use a voice that is:

- **Clear and direct** — Front-load the status or action.
- **Confident and calm** — Do not dramatize downtime, failures, or maintenance.
- **Helpful** — Give the next useful action whenever one exists.
- **Technical when needed** — Preserve terms users need to diagnose or operate the service.
- **Gaming-friendly, not gamer-slang heavy** — Sound modern and familiar without forcing memes, hype, or edgy language.

Read [references/gaming-voice-and-tone.md](references/gaming-voice-and-tone.md) when defining product voice or reviewing tone across a flow.

## English and Thai

Treat English and Thai as sibling product copy, not as literal source and translation.

- Preserve the same user intent, technical meaning, state, and action.
- Rewrite Thai naturally instead of mirroring English syntax.
- Keep established technical nouns in English when Thai users commonly expect them.
- Do not force a Thai translation for terms such as Server, Console, Backup, Mod, Plugin, Node, RCON, API, CPU, RAM, or DDoS when translation would reduce clarity.
- Prefer concise Thai UI wording. Omit unnecessary pronouns and filler.
- Avoid formal Thai patterns such as "ไม่สามารถดำเนินการ..." when a shorter natural form is accurate.
- Do not append "ครับ/ค่ะ" to routine interface strings. Use politeness only where the product context genuinely calls for it.

Read [references/thai-localization.md](references/thai-localization.md) for bilingual rules and examples.

## Gaming and server terminology

Use one term for one product concept. Do not alternate synonyms merely for style.

Examples:
- **Server** — a game server the customer operates.
- **Instance** — use only when the product actually exposes instances as a separate concept.
- **Node** — physical or virtual host infrastructure; do not call it a server when users must distinguish the two.
- **Restart** — stop and start the same service/server.
- **Reinstall** — reinstall software or rebuild the game-server environment; never use as a synonym for restart.
- **Reset** — return a setting or configuration to a defined default.
- **Wipe** — remove game/world/player data when that is the product's established action.
- **Backup** — a recoverable saved copy. Do not promise recoverability unless the system guarantees it.
- **Console** — live command/output interface, not a generic dashboard.
- **Online / Offline** — use only when they accurately represent reachability or running state.

Read [references/gaming-terminology.md](references/gaming-terminology.md) before creating or auditing copy that contains server, infrastructure, networking, billing, moderation, or community terms.

## Action labels

Use specific verb-first labels.

Prefer:
- Start server
- Stop server
- Restart server
- Create backup
- Restore backup
- Save changes
- View console
- Copy IP address
- Renew subscription
- Join Discord

Avoid generic labels when context is not visible to assistive technology:
- Submit
- OK
- Confirm
- Continue
- Click here

Short labels such as **Start**, **Stop**, or **Restart** are acceptable when the surrounding component already names the server and the action remains unambiguous.

## Server states

State labels should describe the system, not instruct the user.

Prefer:
- Starting
- Running
- Restarting
- Stopping
- Offline
- Updating
- Backing up
- Restoring
- Maintenance
- Unavailable

Do not present an in-progress state as completed. Do not use "Online" merely because the control panel is reachable if the game process is still starting.

For detailed state, action, and recovery patterns, read [references/gaming-ui-patterns.md](references/gaming-ui-patterns.md).

## Errors and recovery

An error should answer, when known:

1. What failed?
2. What useful cause or constraint is known?
3. What can the user do next?

Pattern:

`[Action/state failed]. [Useful cause]. [Recovery action].`

Good:
- **Server failed to start. Check the console for the latest error.**
- **Backup failed. There isn't enough storage available. Free up space and try again.**
- **Connection lost. Reconnect to continue viewing the console.**

Avoid:
- Something went wrong.
- An unexpected error occurred.
- Operation failed.
- Error 500.

Keep error codes when they help support or troubleshooting, but pair them with human-readable copy.

Never invent a cause. If the system does not know why an action failed, say what is known and point to the next diagnostic or recovery step.

## Destructive and high-risk actions

Be explicit when an action can cause downtime, data loss, billing impact, access loss, or irreversible changes.

For confirmations:
- Name the action in the title.
- State the consequence before the primary action.
- Identify what is preserved and what is removed when relevant.
- Use the exact destructive action as the primary button label.
- Do not use fear, guilt, or dark patterns.

Example:

**Wipe server data?**

This removes the current world and player data. Server settings are kept.

[Cancel] [Wipe server data]

Use [references/gaming-ui-patterns.md](references/gaming-ui-patterns.md) for restart, reinstall, wipe, restore, cancellation, and permission patterns.

## Maintenance and incidents

Write operational notices in this order:

1. Current impact
2. Scope
3. User action, if any
4. Next update or recovery state, only when known

Prefer:
- **Server controls are temporarily unavailable during maintenance. Running servers are not affected.**

Avoid:
- **We're currently experiencing an unforeseen technical issue and sincerely apologize for any inconvenience caused.**

Do not claim an ETA, root cause, or fix until known.

## Billing and subscriptions

Use exact billing terms and separate access state from payment state.

Distinguish:
- Payment failed
- Payment pending
- Subscription expired
- Subscription canceled
- Renewal scheduled
- Service suspended
- Refund requested / processed

Do not say "Your server was deleted" if the actual state is suspended or retained for a grace period.

Surface dates, retention windows, and consequences when they affect the user's decision.

## Empty states and onboarding

Empty states should explain what is missing and provide the next useful action.

Good:
- **No servers yet**  
  Create your first server to get started.  
  [Create server]

- **No backups yet**  
  Create a backup before making major changes.  
  [Create backup]

Do not add motivational filler that delays the action.

For onboarding, teach the minimum needed for the next successful step. Avoid long welcome copy before users can do anything.

## Community and player-facing features

For whitelist, queue, bans, reports, Discord, roles, or player management:
- Use neutral, factual wording.
- Separate status from judgment.
- Show duration and scope for temporary restrictions when available.
- Do not expose private moderation notes to players unless intentionally designed for that audience.
- Avoid joking language in enforcement, appeals, payments, or account access.

## Accessibility

- Keep visible labels meaningful without relying on icons or color.
- Write descriptive links.
- Pair field errors with the affected field.
- Do not communicate server health only with green/red indicators.
- Make destructive actions distinguishable by wording, not color alone.
- Preserve technical identifiers when screen-reader users may need to copy them.

Read [references/accessibility-guidelines.md](references/accessibility-guidelines.md) for the full accessibility checklist.

## Workflow

1. Identify the user's goal and the system state.
2. Identify the UI surface: button, label, status, error, modal, toast, form, onboarding, billing, or announcement.
3. Preserve technical facts and product terminology.
4. Draft the shortest version that still lets the user act correctly.
5. Adapt tone to risk and emotional context.
6. For TH/EN, localize intent instead of translating sentence structure.
7. Check accessibility and destructive-action clarity.
8. If reviewing a flow, check terminology and state consistency across every screen.

## Review checklist

Before finalizing copy, verify:

- Does the string describe the correct system state?
- Is the next action obvious when action is possible?
- Is any cause presented as fact actually known?
- Are destructive consequences explicit?
- Is terminology consistent?
- Would the Thai version sound natural to a Thai user?
- Would the English version sound like product UI rather than documentation?
- Can a screen-reader user understand the action without visual context?
- Did we avoid hype, slang, corporate filler, and translation-like wording?

## Resources

Load only what is relevant:

- [references/gaming-voice-and-tone.md](references/gaming-voice-and-tone.md) — product voice and tone by situation.
- [references/gaming-ui-patterns.md](references/gaming-ui-patterns.md) — server states, destructive actions, errors, billing, maintenance, and community patterns.
- [references/gaming-terminology.md](references/gaming-terminology.md) — canonical game-server and hosting terminology.
- [references/thai-localization.md](references/thai-localization.md) — Thai/English localization rules and examples.
- [references/accessibility-guidelines.md](references/accessibility-guidelines.md) — accessibility guidance.
- [references/content-usability-checklist.md](references/content-usability-checklist.md) — optional structured UX-copy review.
- [templates/error-message-template.md](templates/error-message-template.md) — detailed error template.
- [templates/empty-state-template.md](templates/empty-state-template.md) — empty-state template.
- [templates/onboarding-flow-template.md](templates/onboarding-flow-template.md) — onboarding template.
