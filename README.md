# ChatGPT Image Automation — selector config

Runtime configuration for the
[ChatGPT Image Automation](https://chrome.google.com/webstore) Chrome extension.

This repository is public on purpose. The extension fetches `selectors.json`
from here so that when ChatGPT changes its page structure, the fix is a commit
to this file rather than a new Web Store submission and a multi-week review.

**Data only.** CSS selector strings, word lists and timeouts. No executable
code is served from here, and none ever should be — remotely hosted code
violates Chrome Web Store policy.

## Fixing a broken selector

1. Open ChatGPT and inspect the element that stopped matching.
2. Add the new selector at the **top** of that key's list (they are tried in
   order — leave the old ones below for users on older builds).
3. Bump `version`.
4. Commit and push to `main`.

Installed copies pick it up within the hour, and immediately on browser restart.
