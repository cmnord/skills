---
name: help-me-do-this
description: Do as much of a task as possible yourself, then give the user only the remaining steps, with exact links, commands, and ready-to-send messages. Use when the user says "help me do this," asks how to accomplish something, or wants their manual work minimized, including steps they will forward to someone else.
---

# Help Me Do This

Complete as much of the task as possible for the user. Give the user only the remaining steps they must perform.

## Required order

Use these methods in order. Move to the next method only when the earlier methods cannot complete the task.

1. Do the work directly with the available tools and access.
2. If access, approval, authentication, or a missing integration is the only blocker, request exactly what is needed so the agent can continue and do the work itself.
3. Provide terminal commands for the user to run.
4. Provide click-by-click steps with direct links.
5. Provide click-by-click steps without links only when a reliable direct link is unavailable.

Do not offload work the agent can perform. Do not present lower-priority methods as alternatives when a higher-priority method succeeds. Never claim an action succeeded without verifying it.

## User steps

When user action remains:

- Give one numbered list in execution order.
- Put prerequisites before the action that needs them.
- State what the user should expect after each consequential step.
- Use the fewest steps that still name every control and value.
- Omit background, optional variations, and already completed work unless needed to avoid a mistake.
- Keep copyable values, commands, URLs, and messages exact.

Treat every terminal command as running in a brand-new terminal opened at its default directory. Make each command block self-contained: start with an explicit `cd` to the required absolute directory when location matters, include required environment setup, and do not rely on state from an earlier command block. Explain placeholders before the block and avoid commands that expose secrets.

For click operations, link directly to the most specific destination available. Use descriptive Markdown link text, name the exact controls to click, and mention visible labels the user can verify. If no stable direct link exists, identify how to navigate there from the product's home screen.

## Help from other people

If another person must grant access, approve something, supply information, or perform an action, include a ready-to-send message at the relevant numbered step. Keep it short and clear:

> Hi [name] - please [specific action] for [resource/project] so I can [outcome]. [Direct link, if available]. Thanks.

Replace placeholders with known details. Ask only for unknown details that are necessary to send the message.
