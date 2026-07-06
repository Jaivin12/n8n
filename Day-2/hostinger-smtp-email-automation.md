# Day 2 - SMTP Email Automation with n8n

## Objective

The goal of Day 2 was to learn how to send automated emails using n8n with an SMTP email account.

This day focused on building a basic email automation workflow that can send emails one by one with a delay between each email.

---

## What I Worked On

- Connected an SMTP email account with n8n
- Created a new email automation workflow
- Built a simple recipient list using a Code node
- Used Loop Over Items to process recipients one by one
- Added a Wait node to create a delay between emails
- Created an HTML email template
- Tested email delivery using sample recipients
- Removed the default n8n attribution footer from the email
- Checked how sender name and sender email appear in Gmail
- Learned the difference between test sending and production campaign sending

---

## Workflow Structure

```text
Manual Trigger
      ↓
Code Node
      ↓
Loop Over Items
      ↓
Send Email
      ↓
Wait
      ↓
Loop Over Items


## Nodes Used

| Node | Purpose |
|---|---|
| Manual Trigger | Starts the workflow manually |
| Code Node | Holds sample recipient data |
| Loop Over Items | Sends one email at a time |
| Send Email | Sends email using SMTP |
| Wait | Adds delay between emails |


Important Expressions
To Email: {{ $json.email }}
Name: {{ $json.name }}
Delay Setup
Wait Time: 10 seconds

So yes: **workflow, nodes, commands, expressions, folder structure = grid/code block/table**.  
Normal explanation can stay as normal markdown.