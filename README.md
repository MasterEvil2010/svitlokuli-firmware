# LightBalls / Світлокулі — Firmware Releases

Public release channel for signed ESP8266 firmware used by the **Світлокулі (LightBalls)** controllers.

## Download

Open the [Releases](https://github.com/MasterEvil2010/svitlokuli-firmware/releases) page and choose the latest stable firmware release.

Each release contains:
- `NodeMCU_Balls_Main.bin.signed` — signed ESP8266 firmware for OTA.
- `firmware.json` — release version, firmware size, and SHA-256 checksum.

## Signature verification

Firmware binaries are signed with **RSA-2048 / SHA-256**. Controllers have the corresponding **public key** embedded in their firmware and reject unsigned or modified OTA binaries. The private signing key is stored offline on the maintainer's Mac; it is **never included in this public repository**.

**Do not use an unsigned `.bin` for OTA after signature verification has been enabled.**

The source code and signing tools are maintained separately in a private repository.
