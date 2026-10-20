# HT5290 Network Radio Introduction

<img width="2364" height="1773" alt="HT5290_图1_正面精修_白底" src="https://github.com/user-attachments/assets/cc2ddbfd-ea3b-4abe-aba2-832c4f466313" />


1. **Network / Radio**: WiFi network radio, favorites, playback
2. **FM / Radio**: FM, LW long wave, MW medium wave, SW shortwave, OIRT, AIR aviation band, with SSB/CW reception support
3. **System / Settings**: language, timer, WiFi, brightness, lock screen, theme, factory reset, and related settings
4. **Computer / Sound Card**: USB sound card mode; entering this mode restarts the device
5. **PC / Configuration**: USB configuration mode for reading and writing parameters through a PC tool; entering this mode restarts the device
6. **Weather / Meteorology**: check weather online via network; requires city or location configuration
7. **Clock / Calendar**: time, perpetual calendar, NTP auto-sync, time zone settings
8. **SSB / CW**: single-sideband reception, Morse CW decoding, CW key practice
9. **Voice Prompt Broadcast**: supports Chinese and English announcements

# Network / Radio

Network radio requires a 2.4G WiFi connection.

- Volume range: 0-30, default 20
- Volume is stored independently from the radio volume
- Playback states: playing, buffering, connected, paused, playback error
- Menu includes: station list, my favorites, last 5 played, sound effects, background playback
- Two ways to add radio stations:
  1. Connect to the device hotspot `HT5290-NetRadio` with password `12345678`, then visit `http://192.168.4.1`; up to 10 stations can be added
  2. Use the PC configuration tool; up to 1000 stations can be written at one time, and the device supports up to 1500 total stations
- Supports direct MP3 stream links via HTTP/HTTPS, including Qingting and other live-streaming URLs
- A single URL can be up to 192 characters long
- Supports playback of other stream sources through the "CanPlay" software on a PC, which bridges unsupported audio links such as `.aac`, `.m4a`, `.wav`, `.ogg`, and `.m3u8` and routes them to the radio over WiFi

# CanPlay Software

1. The radio cannot natively play formats such as `.aac`, `.m4a`, `.wav`, `.ogg`, and `.m3u8` in the same way as Android or other systems. During playback, these formats may stutter or be blocked, so only smooth MP3 streaming is retained for direct playback.
2. When such audio files need to be played, use the "CanPlay" software on a PC. Run the software on a computer, copy the playable stream link into the software, create a custom channel number and a single playback URL, then import the channel number and URL into the radio using a phone or PC configuration tool. The radio can then listen normally through the configured channel.

# Smart Clock and Weather System

- NTP auto time synchronization, perpetual calendar, supports 12/24-hour time format
- Built-in clock chip keeps accurate time automatically after WiFi or manual time setting; power-loss memory support
- Weather is obtained online: in China, a 9-digit city code can be entered; overseas users can set English place names or latitude/longitude; temperature, humidity, wind force, and other weather information are displayed
- Timed power on/off is supported: daily scheduled power on/off; scheduled power-on can directly play FM or network radio after wake-up

# WiFi Setup

- Only supports 2.4GHz WiFi, not 5G
- Up to 3 WiFi networks can be saved; the 4th will overwrite the earliest saved network
- Example saved networks: home, office, mobile hotspot
- Device hotspot name: `HT5290-NetRadio`
- Password: `12345678`
- Configuration page address: `192.168.4.1`
- Configuration entry: System Settings → WiFi Settings → Network Connection
- Network radio, weather, and NTP auto-sync all rely on WiFi
- WiFi can also be configured through PC software by selecting the WiFi name and entering the password

# System / Settings

1. Language: supports 21 languages
2. Timer: scheduled power on/off, wake-up audio selection, FM or network radio
3. WiFi: WiFi switch and network connection
4. Brightness: display brightness adjustment
5. Lock screen: screensaver brightness and timeout
6. Theme: custom display color settings
7. Voice prompt: announcement language switch
8. Factory reset and other system operations

# FM / Radio / Aviation / Single Sideband / CW Decoding

FM receive sensitivity: -90 dBm to -99 dBm

Band frequency range notes:

- FM (ordinary FM): 87-108 MHz, supports RDS
- Long press the knob to read RDS text
- Stereo and de-emphasis settings
- OIRT (Eastern European FM): 64-75 MHz
- Old Eastern European FM broadcasts; also supports RDS/RBDS
- LW long wave: 153-279 kHz
- MW medium wave: 522-1701 kHz
- SW shortwave: 2.3-26.1 MHz
- SSB/CW operates within this shortwave range
- Switch to SSB/CW mode for LSB/USB sideband + BFO beat frequency

## AIR Aviation Band (VHF Airband)

- Frequency: 108-137 MHz
- Step size can be switched:
  - China mode: 25 kHz
  - Europe mode: 8.33 kHz

> Note: Aviation band is receive-only and does not support transmission.

## SSB / CW (Single Sideband and Morse Code Reception)

> Warning: SSB and CW do not have independent hardware frequency bands. They share the SW shortwave range from 2.3-26.1 MHz. The single-sideband demodulation mode is enabled only when entering the SSB/CW function menu.

### SSB Reception

- Available sidebands: LSB and USB
- Frequency range: 2.3 MHz to 26.1 MHz
- Adjustable parameters: BFO beat frequency, bandwidth, frequency step, beat-step; screen shows signal strength and SNR; long-press numeric input is supported for frequency entry

### CW (Morse Code)

1. **CW decoding (receive mode)**: uses the same 2.3-26.1 MHz range to receive Morse signals from the air; the screen directly translates the code into text; adjustable WPM rate, threshold, and tone
2. **CW practice (local mode)**: connect an external key to practice sending locally; this is not air reception and does not occupy external radio frequencies; adjustable dash/dot threshold, character spacing, debouncing, prompts, and volume

### Useful Tips

1. When listening to weak shortwave, SSB, or CW signals, it is recommended to turn off WiFi because WiFi can introduce interference noise.
2. In FM/OIRT mode, long-press the knob to display RDS. In SSB mode, adjust the BFO beat frequency to clarify the single-sideband voice.
3. All band station storage limit: the search list supports up to 500 entries.

# Computer / Sound Card

1. Use the supplied USB charging cable to connect to a computer; the radio enters computer sound card mode and plays the computer audio output.
2. When entering computer sound card mode, the system may show a black screen and restart; this is normal.

# PC / Configuration

1. Mainly used to upload network radio station lists, batch upload up to 1000 entries, configure network settings, weather settings, WiFi configuration, upload custom boot logo, and update firmware.
2. Put the radio into PC configuration mode; entering this mode may cause a black screen and restart. Then open the PC software and select the device with the USB connection.

# Weather / Meteorology

1. Users can connect through a phone to the WiFi configuration interface, enter the local city weather ID in the weather field, and then obtain local weather information. If location is not detected, check whether the phone has location permission enabled. If needed, disable location restrictions or ask a large language model such as Doubao for your city weather ID (for example: "What is the weather ID for Shenzhen?").
2. Overseas users need to enter coordinates (latitude/longitude) in the mobile interface or PC software to obtain weather information; the system will automatically display the city name.

# Clock / Calendar

1. Supports global clock display, manual time correction, or automatic correction via WiFi. After synchronization, the clock continues to operate while in standby or after power is removed.
2. Enter settings to adjust other clock parameters.
3. You can set scheduled power on/off times in the system settings and specify the startup audio, such as FM 99.9 MHz or a network radio station.

# Language Prompt / Custom Logo

1. Increases the playability of the device and provides reminders and guidance for players who do not find the operation convenient. After enabling it, the operation becomes slower; in the system settings, turning off the voice prompt simplifies the workflow.
2. Users can create a 320x240 image and upload it via computer to change the startup screen.

# Single Sideband / CW Decoding / CW Practice

1. Single sideband is divided into upper sideband and lower sideband. Normally it cannot receive radio stations like FM at all times; it requires a specific device or the presence of other players transmitting SSB signals, or you may have your own device.
2. CW decoding converts received Morse radio waves into readable code. The decoding structure is for reference only and is intended for entertainment and learning; it should not be treated as an exact real-world result and the result should be verified by the user.
3. CW sending practice converts keying technique into readable results, turning dots and dashes into displayed output. It does not provide real transmission capability and is mainly used to practice keying technique.
