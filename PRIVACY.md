# Privacy Policy — TabWatch

**Last Updated:** November 2026

TabWatch is built with a local-first architecture. Most features operate entirely inside your browser without communicating with any external server.

## 1. Local Browser Data
- Your monitoring rules, keywords, autostart URL patterns, refresh intervals, audio/TTS preferences, and match history are stored **locally on your device** using `chrome.storage.local`.
- Webpage contents scanned by TabWatch's keyword and DOM observer are processed locally in memory and are **never** transmitted to external servers for general monitoring.

## 2. Pro Cloud Email Alerts (Opt-In)
If you subscribe to TabWatch Pro and explicitly verify a recipient email address:
- **Email Verification:** Your email address, license key, and local `instanceId` are sent to our alert webhook (`/api/send-verification` and `/api/verify-code`) to deliver a 6-digit verification code.
- **Match Notifications:** When a rule with email alerts enabled triggers, only the verified recipient email, license key, `instanceId`, matched keyword, event type (`Found` / `Lost`), page URL, short text snippet, and timestamp are sent to `/api/send-alert` to deliver your notification email.

## 3. License Key & Billing (Polar.sh)
- Subscription checkout, billing management, and license key activation/validation (`activate`, `validate`, `deactivate`) communicate directly with **Polar.sh** (`api.polar.sh`).
- TabWatch does not collect, process, or store your credit card or payment details.

## 4. Data Retention & Control
You can pause or delete any monitoring rule, clear your match history, deactivate your device license key, or uninstall the extension at any time to remove local data.

## 5. Contact
For privacy questions or support requests, contact: `donj73w@gmail.com`
