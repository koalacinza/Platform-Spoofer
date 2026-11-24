# Platform-Spoofer

**Platform-Spoofer** allows you to configure how your platform is identified on Discord via BetterDiscord. You can select one or multiple options, such as **PC + mobile** or **PC + console**.

### What can you select?

- **PC** — Windows client
- **Browser** — Web version
- **Mobile** — Discord for Android
- **Meta Quest** — VR identification
- **Console** — PlayStation identification

The options are independent: select only the ones you want, or use the **Select all** and **Deselect all** buttons. Your choices are saved and applied via an automatic reconnection—no need to restart Discord.

## How to install

1. Place the `Platform-Spoofer.plugin.js` file into your BetterDiscord plugins folder.
2. In Discord, go to **Settings → BetterDiscord → Plugins** and enable **Platform-Spoofer**.
3. Open the plugin settings and choose your platforms.

The plugins folder location depends on your operating system:

```text
Windows  %appdata%\BetterDiscord\plugins
Linux    ~/.config/BetterDiscord/plugins
macOS    ~/Library/Application Support/BetterDiscord/plugins
```

## Checking via the console

If you want to verify your selection or trigger a new connection, open the Discord developer console and use:

```js
__ps.status();     // Selected platforms and connection status
__ps.sessions();   // Sessions accessible to the client
__ps.reconnect();  // Force a new connection
```

> **Warning:** This is an unofficial plugin that modifies how Discord handles connections. Its use may violate the platform's Terms of Service. Use at your own risk.
