# HT5290 Network Radio Introduction

## 1. Network / Radio

- Network radio: WiFi network radio, favorites, playback
- FM / radio: FM, LW long wave, MW medium wave, SW shortwave, OIRT, AIR aviation band, with SSB/CW reception support
- System / settings: language, timer, WiFi, brightness, lock screen, theme, factory reset, and related settings
- Computer / sound card: USB sound card mode, entering this mode will restart the device
- PC / configuration: USB configuration mode, used for reading and writing parameters through a PC tool; entering this mode will restart the device
- Weather / meteorology: view weather online after connecting to the network; requires city or location configuration
- Clock / calendar: time, perpetual calendar, NTP auto-sync, time zone settings
- SSB / CW: single-sideband reception, Morse CW decoding, CW key practice
- Voice prompt broadcast: supports Chinese and English announcements

## 2. Network Radio

Network radio requires a 2.4G WiFi connection.

- Volume range: 0-30, default 20
- Volume is stored independently from radio volume
- Playback states: playing, buffering, connected, paused, playback error
- Menu includes: station list, my favorites, last 5 played, sound effects, background playback
- Two ways to add stations:
  1. Connect to the device hotspot `HT5290-NetRadio` with password `12345678`, then visit `http://192.168.4.1`; up to 10 stations can be added
  2. Use the PC configuration tool; up to 1000 stations can be written at one time, and the device supports up to 1500 total stations
- Supports direct MP3 stream links via HTTP/HTTPS, including live addresses from Qingting and other services
- Single URL length supports up to 192 characters
- Supports playback of audio streams that are not natively supported by the radio by using external bridge software on a PC and routing the stream to the device through WiFi

## 3. Playable Software

The radio system cannot natively play certain formats such as `.aac`, `.m4a`, `.wav`, `.ogg`, and `.m3u8` like Android or other operating systems. During playback, these formats may stutter or be blocked, so only smooth MP3 streaming is retained for direct playback.

If you need to play such audio files, you can use the "CanPlay" software on a PC.

- Run the software on a computer
- Copy the playable stream link into the software
- Assign a custom channel number and a single stream URL
- Import the channel number and URL into the radio through a mobile app or PC configuration tool
- Then the radio can play normally through the configured channel

This method allows audio streams that the radio cannot decode directly to be bridged to the home router or WiFi network and then accessed by the radio as normal channels.

## 4. Smart Clock and Weather System

- NTP auto time synchronization
- Perpetual calendar support
- 12/24-hour time format support
- Built-in clock chip keeps accurate time after WiFi or manual setup; power-loss memory is supported
- Online weather retrieval via network
- Domestic support: 9-digit city code input
- International support: English city names / latitude and longitude input
- Displays temperature, humidity, wind strength, and other meteorological information
- Scheduled power on/off support
- Daily scheduled power on/off is supported
- Scheduled power-on can choose to directly play FM or network radio after wake-up

## 5. WiFi Configuration

- Only supports 2.4GHz WiFi, not 5G
- Maximum of 3 WiFi profiles can be saved; the 4th profile will overwrite the oldest saved network
- Example saved networks: home, office, mobile hotspot
- Device hotspot name: `HT5290-NetRadio`
- Password: `12345678`
- Configuration page address: `192.168.4.1`
- Configuration entry: System Settings → WiFi Settings → Network Connection
- Network radio, weather, and NTP time synchronization all depend on WiFi
- WiFi can also be configured through PC software by selecting the WiFi name and entering the password

## 6. System / Settings

1. Language: supports 21 languages
2. Timer: scheduled power on/off, wake-up audio selection, FM or network radio
3. WiFi: WiFi switch, network connection
4. Brightness: display brightness adjustment
5. Lock screen: screensaver brightness and screensaver timeout
6. Theme: custom display color settings
7. Voice prompts: announcement language switch
8. Factory reset and related system operations

## 7. FM / Radio Features

The radio system supports multiple band modes and reception functions, including:

- FM
- LW long wave
- MW medium wave
- SW shortwave
- OIRT
- AIR aviation band
- SSB reception
- CW reception

This makes the device suitable for both standard broadcast listening and advanced radio practice.

## 8. SSB / CW

The SSB/CW module provides:

- Single-sideband reception
- Morse CW decoding
- CW key training practice
- Advanced tuning support for radio communication and learning scenarios

## 9. Voice Prompt Broadcast

The system supports voice prompts in:

- Chinese
- English

This feature improves usability and allows users to receive audio feedback for settings, playback status, and system actions.

## 10. Summary

The HT5290 network radio is a multifunctional internet-enabled radio device designed for modern listening, configuration, and radio practice. It combines network radio playback, FM/LW/MW/SW reception, SSB/CW support, weather and clock functions, WiFi networking, and voice announcement features in a single platform.

It is suitable for:

- Daily radio listening
- Shortwave and SSB exploration
- Morse code practice and CW learning
- Network radio streaming
- Weather and time synchronization features
- Smart home-style radio device usage

This design balances user-friendly control, feature-rich radio operation, and practical embedded-device functionality.

