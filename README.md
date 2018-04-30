# Home Assistant Configuration

## Screenshot

![UI](hass.png)

## Setup
- Synology DS415+ *(running synology docker)*
- [Home Assistant](https://home-assistant.io/)

## Things
- Plex Media Server *(currently running via nvidia shield)*
- Philips Hue lights (hue tap & motion sensor via custom component)
- Sonos
- [Tado Smart Thermostat](https://www.tado.com/gb/)
- Nvidia Shield TV *(running plex server & client, cast, kodi, emby)*

## Presence
- Asuswrt, Bluetooth & Tado device tracking
- Bayesian Binary Sensor provides probability based logic which seems to >
  make presence detection more accurate

## Automations
Plex
- Activate native hue scene (living room movie) when movie playing in cast/plex/emby/kodi
- Activate native hue scene (living room full) when movie stopped or paused in cast/plex/emby/kodi
- Activate native hue scene (living room dim) when tvshow playing in cast/plex/emby/kodi
- Activate native hue scene (living room full) when tvshow stopped or paused in cast/plex/emby/kodi
- Pause sonos speakers when cast/plex/emby/kodi starts playing

Lights
- Turn lights on around sunset (inside & out)
- Turn inside lights off at bedtime
- Turn outside lights off in the morning

Notifications
- Send pushover notification if home-assistant restarts
- Send pushover notification if home-assistant has an update available
- Send pushover notification if certain docker containers are not running

Telegram Bot
- Interact with home assistant with telegram bot commands

Various
- Guest mode - turns off certain automations if we have guests over (i.e. we *might* have to stay up later than 22:15!)
