---
permalink: /privacy/
title: "Privacy Policy"
---

# Privacy Policy

**Last updated:** June 2, 2026

This privacy policy applies to the Google OAuth application "Kou's Workspace" (the "Application"), which is used by Zili KOU to access Google Workspace services (Gmail, Calendar, Drive, Sheets, Docs) via the Hermes Agent personal automation system.

## Information We Access

The Application requests access to the following Google services, limited to data associated with the authorized Google account (kouzili9777@gmail.com):

- **Gmail** — read, modify labels, and send email on behalf of the user
- **Google Calendar** — read, create, and delete calendar events
- **Google Drive** — read, create, and modify files
- **Google Sheets** — read and write spreadsheet data
- **Google Docs** — read and write document content
- **Contacts** — read contact information

## How We Use the Information

All data accessed by the Application is used **only** for personal automation tasks performed by the account owner. Specifically:

- Reading and sending emails on behalf of the account owner
- Reading and creating calendar events for the account owner
- Reading and modifying Drive files owned by the account owner
- Reading and writing Sheets and Docs owned by the account owner
- Reading contacts for the account owner's personal use

The Application does **not**:

- Transfer any user data to any third party
- Use any user data for advertising, marketing, or commercial purposes
- Use any user data for training artificial intelligence models
- Sell, lease, or share any user data with any other party

## Data Storage and Security

- OAuth access tokens and refresh tokens are stored locally on a personal device owned by the account owner, in a file at `~/.hermes/google_token.json` (Linux/macOS) or `%USERPROFILE%\.hermes\google_token.json` (Windows).
- Token files are protected by the operating system's standard filesystem permissions (readable only by the account owner).
- The Application does not transmit, sync, or back up token files to any external server.
- All API calls are made directly from the account owner's device to Google's API endpoints (`googleapis.com`).

## Data Retention

- API responses are processed in-memory and are not retained by the Application beyond the duration of the relevant automation task.
- Token files persist on the account owner's device until manually revoked (`setup.py --revoke`) or until the OAuth consent is revoked via the user's Google account settings.

## Revoking Access

The account owner can revoke the Application's access at any time via:

1. Google's account security page: <https://myaccount.google.com/permissions>
2. Or by running the command `python setup.py --revoke` from the Application's installation directory

After revocation, the Application will no longer be able to access any Google service on the account owner's behalf.

## Contact

For any questions about this privacy policy, contact:

**Zili KOU**
Email: kouzili9777@gmail.com
Website: <https://kouzili.github.io/>

## Changes to This Policy

This privacy policy may be updated from time to time. The "Last updated" date at the top of this page reflects the most recent change.
