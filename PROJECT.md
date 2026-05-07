# DEVGRU MC - Support Board Guide

This document describes how the admin team uses the GitHub Project board to manage support tickets.

## Board Columns

### Triage
All newly opened tickets land here automatically. An admin should review and move them within 24-48 hours.

**Admin action:** Read the ticket. If valid, decide the priority and move it to Backlog or In Progress. If duplicate or invalid, close it with a comment explaining why.

### Backlog
Tickets that are acknowledged and legitimate but not being actively worked yet. The user has been seen, they just have to wait. Remove the `triage` label and add `backlog`.

**Admin action:** Leave a comment letting the user know their ticket is in the queue. Move to In Progress when you're ready to pick it up.

### In Progress
An admin has picked up the ticket and is actively working on it. Assign yourself to the issue and swap the label to `in-progress`.

**Admin action:** Update the ticket with progress notes. If you need more info from the user, add the `waiting-on-user` label and move the card to the Waiting on User column.

### Waiting on User
The ball is in the user's court. We're waiting on more information, confirmation, or them to test a fix.

**Admin action:** If the user responds, move back to In Progress. If no response for 7 days, the stale bot will flag it automatically.

### Resolved
Ticket is done. Close the issue and apply the `resolved` label. Leave a closing comment summarizing what was done so there's a record.

## Tips for Admins

- Always leave a comment when moving a ticket - users don't see board movements, only comments
- Use `urgent` label for anything that's actively breaking the server or blocking multiple people
- Don't close tickets silently - a one-line "Fixed in last restart, should be good now" goes a long way
- The Project board must be set up manually in GitHub UI (Settings > Projects on the repo). Create a new board and add the five columns above
