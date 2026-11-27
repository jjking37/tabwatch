# TabWatch — Smart Auto-Refresh & Keyword Monitor

**TabWatch** is a lightweight desktop browser extension (Chrome Manifest V3) for webpage auto-refreshing, live keyword and DOM change monitoring, local audio/TTS alerts, and optional Pro cloud email notifications.

Designed for general-purpose productivity—such as watching public inventory pages, appointment portals, status dashboards, and live listings—TabWatch keeps all monitoring rules and page checks strictly local in your browser.

---

## Key Features

### Free Tier (100% Local Browser Execution)
- **Smart Auto-Refresh & Jitter:** Fixed intervals (including decimals like `0.5s` or `12s`) or randomized jitter ranges (e.g., `15s – 40s`), plus pause-while-typing protection.
- **Keyword & DOM Change Monitor:** Watch for keywords or regular expressions **Appearing (Found)** or **Disappearing (Lost)** with configurable deduplication cooldowns and a local Alerted Tabs History log.
- **Navigation & HUD Polish:** Optional floating countdown HUD pill, automatic scroll restoration, silent reloads without form-resubmission prompts, redirect locking, and system keep-awake (`chrome.power`).
- **Offscreen Audio Chimes & Voice (TTS):** Built-in Web Audio chimes (`1s` ping, `5s` urgent tone, or custom audio URL) and Web Speech API (`speechSynthesis`) announcements that play reliably even when the popup is closed.
- **Autostart & Presets:** Wildcard URL autostart rules and one-click JSON preset import/export.

### TabWatch Pro (Polar.sh Subscriptions)
- **Pro Monthly:** **$2.99 / month** (recurring, cancel anytime via Polar customer portal)
- **Pro Annual:** **$19.99 / year** (recurring, cancel anytime via Polar customer portal)
- **Verified Cloud Email Alerts:** Verify your recipient email with a 6-digit code and receive instant email notifications via our webhook when a monitored keyword matches while you are away from your desk.
- **Multi-Device License Keys:** Managed securely via Polar.sh license keys (up to 3 activated browser instances per key).

---

## Local Installation (Chrome)

1. Open `chrome://extensions` in Google Chrome.
2. Enable **Developer mode** in the top-right corner.
3. Click **Load unpacked** and select this repository root (`tabwatch-chrome/`).

## Packaging for Chrome Web Store

```bash
zip -r -q ../tabwatch-chrome-v1.0.0.zip . -x "cloudflare-worker/*" "docs/*" ".git/*" "README.md" "PRIVACY.md" ".gitignore" ".DS_Store"
```

## Privacy & Support

- **Privacy Policy:** See [PRIVACY.md](./PRIVACY.md).
- **Support Email:** `donj73w@gmail.com`
