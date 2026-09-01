# Privacy Policy — ChatGPT Image Automation

**Last updated: 1 September 2026**

## Summary

This extension does not have a server. It does not collect, transmit, sell or
share your personal data. Everything it stores stays in your own browser.

## What is stored, and where

All of the following is kept in Chrome's local extension storage on your own
machine. None of it is transmitted to us — we operate no backend and have no
way to read it.

| Data | Why | Where it lives |
|---|---|---|
| Your prompt queue and prompt text | To run the batch and resume it after a restart | Your browser only |
| Reference style and character descriptions | To set up consistency before the batch | Your browser only |
| Reference images you attach | To send as the visual reference | Your browser only |
| Folder name and filename prefix | To name downloaded files | Your browser only |
| Licence key and activation status | To unlock PRO features | Your browser only |
| Run status and progress | To resume an interrupted batch | Your browser only |

Clearing the extension's data, or uninstalling it, removes all of it permanently.

## Network requests

The extension makes exactly three kinds of outbound request:

1. **chatgpt.com** — the extension operates the ChatGPT page you already have
   open, in your own logged-in session. It sends the prompts you entered. It
   does not read, collect or transmit your ChatGPT conversations anywhere else,
   and it has no access to your OpenAI credentials.

2. **`*.oaiusercontent.com`** — downloading the images ChatGPT generated for
   you, so they can be saved to your chosen folder.

3. **`raw.githubusercontent.com/shusayn/chatgpt-image-automation`** — fetching
   a small configuration file listing CSS selectors, so the extension keeps
   working when ChatGPT changes its page layout. This request sends no data
   about you: it is an anonymous read of a public file. It contains
   configuration data only, never executable code.

4. **`api.gumroad.com`** — only when you activate or re-verify a PRO licence.
   Your licence key is sent to Gumroad to confirm the purchase is valid. See
   [Gumroad's privacy policy](https://gumroad.com/privacy).

## What we do not do

- No analytics, telemetry, tracking pixels or usage reporting
- No advertising, and no data sold or shared with third parties
- No reading of your browsing history, bookmarks, cookies or passwords
- No access to any site other than `chatgpt.com`
- No account, and no sign-up

## Permissions, and why each is needed

| Permission | Why it is required |
|---|---|
| `storage` | Save your queue, settings and progress locally |
| `downloads` | Save generated images to your chosen subfolder |
| `scripting` | Re-inject the automation script if a ChatGPT tab reloads mid-run |
| `sidePanel` | Show the control panel beside the page |
| `alarms` | Resume a long batch reliably after Chrome suspends the worker |
| `chatgpt.com` | The site the extension automates |
| `*.oaiusercontent.com` | Where ChatGPT serves your generated images |
| `raw.githubusercontent.com/shusayn/...` | Selector configuration, so layout changes do not break the extension |

## Children

This extension is not directed at children under 13.

## Changes

Material changes to this policy will be published here with an updated date and
noted in the extension's release notes.

## Contact

Questions or a data request: **hussain76t45@gmail.com**
