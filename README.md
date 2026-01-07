# Brave Debloat (macOS 26 Tahoe and newer)

This repository provides a configuration profile that disables unwanted built-in features in **Brave Browser** using **system-level managed policies**.

The profile survives Brave updates and enforces settings at the operating system level.

---

## What this profile disables

- Brave AI / Leo / Chat
- Brave Wallet (crypto)
- Brave VPN
- Brave Rewards
- Other optional Brave features controlled via policy

---

## Supported systems

- **macOS 26 Tahoe**
- **macOS 26+ (Tahoe and newer)**

Older macOS versions are not supported by this guide.

---

## Installation (recommended)

Run the following one-liner in Terminal:

```bash
URL="https://raw.githubusercontent.com/dominiaz/brave-debloat/main/brave-debloat.mobileconfig"; OUT="$HOME/Downloads/brave-debloat.mobileconfig"; curl -fsSL "$URL" -o "$OUT" && open "$OUT" && echo -e "\nProfile downloaded to: $OUT\n\nmacOS 26 Tahoe and newer: System Settings -> General -> Device Management -> Pending Profile -> Install\n"
