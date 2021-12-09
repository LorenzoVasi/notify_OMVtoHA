# Notification from OpenMediaVault to Home Assistant

## Requirement

`curl` must be installed into OpenMediaVault system

```
apt install curl
```

## Configuration

There's 3 simple settings into the script:
1. **TOKEN_HA** = Here you must insert the token of your Home Assistant instance. For create it, go to bottom-left corner to username -> Make long life token
2. **URL** = You must insert your URL of your Home Assistant instance. Remember http or https and don't add `/` at the finish of URL
3. **DEVICE** = Here you can insert the device of notification after notify.[DEVICE]

### Example of Configuration

```bash
TOKEN_HA="ASHJBDAISJBDHASJBDFUJKASHFGVBHJSGFSI"
URL="https://www.domain.it:8123"
DEVICE="persistent_notification"
```

## Installation

After install curl on your system, copy the script into this path:
`/usr/share/openmediavault/notification/sink.d/`

You can test it into Notification sub-menu of OpenMediaVault with the botton `SEND A TEST EMAIL` (for enable it, you must add an email (you can write anything you want 👍)
