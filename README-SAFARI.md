# Grok AI Safari iPhone package

1. Host this folder from an HTTPS web server.
2. Open `index.html` via the HTTPS site in Safari on iPhone.
3. Share -> Add to Home Screen -> turn on Open as Web App -> Add.
4. Configure an authenticated `wss://` Grok Build/ACP relay in Settings.

The entire supplied Grok Build source is preserved in `Original-Grok-Build-Source/`.
The browser client adapts the user-facing agent/session/project workflow to Safari.

A browser cannot execute the original desktop Rust agent, arbitrary host shell commands, PTYs, or unrestricted iOS filesystem operations. Those host-specific capabilities remain in the preserved source and are accessed through a trusted remote agent/relay or explicit browser-safe APIs.
