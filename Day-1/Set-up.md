# Day 1 - n8n Installation and First Workflow

## Objective

Set up n8n on my local machine and successfully send my first automated email using Gmail.

---

## System Information

- Operating System: Windows 11
- Node.js Version: v22.23.1
- npm Version: 10.9.8

---

## Installation

Verified Node.js installation:

```bash
node -v
```

Output:

```
v22.23.1
```

Verified npm:

```bash
npm -v
```

Output:

```
10.9.8
```

Installed n8n:

```bash
npm install -g n8n
```

---

## Issue Faced

Running:

```bash
n8n
```

Resulted in:

```
Error: Command "start" not found
```

### Solution

Started n8n using:

```bash
npx n8n
```

This successfully launched the editor.

---

## Accessing n8n

Opened in browser:

```
http://localhost:5678
```

---

## Gmail Integration

Created a Gmail credential.

Granted Google OAuth permissions.

Successfully sent a test email.

Workflow:

Manual Trigger
↓

Gmail Send Email

---

## Key Learnings

- n8n is a workflow automation platform.
- Workflows consist of connected nodes.
- Manual Trigger is useful for testing.
- Gmail node can send emails after authentication.
- Credentials are securely stored by n8n.
- Workflows are saved locally.

---

## Understanding npx

Currently using:

```bash
npx n8n
```

This starts a local n8n server.

The server stops when Command Prompt is closed.

However:

- Workflows remain saved.
- Credentials remain saved.
- Settings remain saved.

To reopen n8n:

```bash
npx n8n
```

Then open:

```
http://localhost:5678
```

---

## Next Goals

- Read contacts from an Excel file
- Send personalized emails
- Process contacts in batches
- Add delays between emails
- Build a complete promotional email campaign workflow