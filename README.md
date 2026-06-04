# GAMERemotePack

GAMERemotePack is a Windows setup helper for playing or checking a PC game from an Android tablet while away from the PC.

It is made for a simple idea: keep the main game running on the home PC, then use an Android tablet to check the screen, chat, craft, gather, manage small tasks, or play lightly from bed or outside the house.

Although it was tested with an MMO-style game workflow, the setup is not limited to one title. If a PC game can be streamed through Sunshine and controlled through Moonlight, the same idea can be used.

## What This Tool Helps With

- Guides the PC setup for Tailscale and Sunshine
- Opens the Sunshine setup screen in an embedded browser
- Guides Android setup for Tailscale and Moonlight
- Creates connection notes for the Android device
- Checks whether Android can see the streamed screen
- Provides input troubleshooting for mouse, tap, keyboard, and controller use
- Includes a keyboard compatibility fix for Sunshine settings
- Explains recommended Moonlight quality settings for home and away use

## Download

Download the latest ZIP from GitHub Releases, extract it, and run:

`BlackAshRemoteSetup.exe`

Releases:
https://github.com/mitaka0715-bot/GAMERemotePack/releases

## Typical Use

1. Keep the home PC powered on.
2. Start the game on the PC.
3. Start Tailscale and Sunshine on the PC.
4. Open Moonlight on Android.
5. Connect to the PC and operate the game screen from Android.

For stable remote use, set Windows sleep to `Never`. Turning the monitor off is usually fine, but PC sleep or hibernation will stop the connection.

## Bed / Hospital / Away-From-PC Use

This pack is useful for light actions where ultra-low-latency play is not required:

- Checking the game screen
- Reading chat
- Sending short chat messages
- Crafting-style repeated tasks
- Gathering-style repeated tasks
- Inventory or menu checks
- Controller-based light play

For serious real-time combat or timing-heavy play, the experience depends heavily on the network connection.

## Recommended Moonlight Settings

Away from home:

- Resolution: 720p
- Frame rate: 30 FPS
- Bitrate: 5 to 10 Mbps
- Codec: H.264 or HEVC

Home Wi-Fi or close-range testing:

- Resolution: 1080p
- Frame rate: 60 FPS
- Bitrate: 20 to 40 Mbps

## Keyboard and Controller Notes

If tap and mouse work but keyboard input does not, check the Android keyboard first. USB keyboards can conflict with the Android device's PC/ADB connection mode. A Bluetooth keyboard is recommended.

Bluetooth controllers can also work through Moonlight/Sunshine. Xbox-style controllers are usually the easiest. The game must be set to gamepad mode if required.

## Important Notes

- This package does not include Tailscale, Sunshine, or Moonlight installers.
- Users install those apps from their official sources.
- Do not open game streaming ports directly to the internet. Use a private VPN-style connection such as Tailscale.
- Account login, Sunshine password creation, and Moonlight pairing must be done by the user.
- No personal tokens, API keys, account credentials, or private IDs are included in this repository.

## Not Affiliated

This project is an independent setup helper. It is not affiliated with any game publisher, Tailscale, Sunshine, or Moonlight.
