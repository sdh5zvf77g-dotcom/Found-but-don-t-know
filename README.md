# Grok AI — iPhone Safari App

GitHub-ready Safari/PWA front end for the iPhone Grok-style coding assistant.

## Deploy with GitHub Pages

1. Create a new GitHub repository.
2. Upload the files in this folder to the repository root.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**, your main branch, and `/ (root)`.
5. Wait for GitHub Pages to publish the site.
6. Open the HTTPS Pages address in Safari on your iPhone.
7. Tap **Share → Add to Home Screen → Open as Web App → Add**.

## What is included

The deployable app contains its complete browser UI, chat client, streaming-message handling, project/file picker, local memory, Autopilot control, settings, PWA manifest and offline service worker.

## Agent connection

Configure an authenticated `wss://` Grok Build/ACP-compatible relay in the app's Settings.

The original desktop Grok Build source is deliberately NOT copied into this web repository. It is kept separately so the GitHub deployment remains small and avoids large/generated/binary repository files.

iOS/Safari cannot directly execute the original desktop Rust agent, unrestricted shell commands or PTY processes. Those capabilities must be provided by a trusted remote agent/relay or replaced with browser/iOS-safe tools.
