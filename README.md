<div align="center">
  <img src="assets/dejisa-logo.png" width="210" />
</div>

# DejiSa 🎵

**A privacy-focused Android music player. Your music. Your sources. Your sound.**

DejiSa is a feature-rich Android music player that brings your music together in one unified library.

Enjoy Plex, Emby and Jellyfin integration, local music, SMB, FTP and SFTP network sources, personalized internet radio, UPnP/DLNA playback, offline downloads, playlists, lyrics, customizable home-screen widgets and Sonic Core DSP.

Connect to Vigilsoni for music recognition, recognition history, artist following, release alerts and concert notifications through ntfy and UnifiedPush.

DejiSa also features customizable Crystal Glass themes, adaptive layouts, local and WebDAV backups, and extensive playback customization.

**One music player. Multiple sources. Your choice.**

## 📱 Screenshots

<p align="center">
  <img src="screenshots/dejisa-home.png" alt="DejiSa home screen" width="46%" />
  <img src="screenshots/dejisa-now-playing-melanite.png" alt="DejiSa now playing screen" width="46%" />
</p>

<p align="center">
  <img src="screenshots/dejisa-advanced-about.png" alt="DejiSa Advanced & About screen" width="68%" />
</p>

*Moonstone and Melanite Crystal Glass themes shown. Screenshots are from DejiSa 3.50.*
---

## 📥 Download

### Latest release: DejiSa 4.00

**[⬇ Download the latest APK](https://github.com/bigtechstruggler/DejiSa-Downloads/releases/latest)**

Download the APK from the release assets and install it on your Android device.

### Requirements

- Android 11 or newer
- Compatible Android device
- Network connectivity for online features

**No Plex, Emby, Jellyfin or other media server is required to play your local music.**

---

## 🎵 One unified music library

Your music should not be limited to a single server, folder or ecosystem.

DejiSa brings music from multiple sources together in one library:

- Local music folders
- Plex Media Server
- Emby Server
- Jellyfin Server
- SMB 2/3 network shares
- FTP servers
- SFTP servers

Browse your music through unified artist, album, track and playlist views, regardless of where your collection is stored.

Additional library features include:

- Source-specific music indexing
- Cached music catalogues
- Artist and album browsing
- Track metadata and artwork
- Unified playback queues
- Locally managed playlists

Your music collection remains organized even when different sources are involved.

---

## 🌐 Network music

DejiSa supports several ways to access music stored on your home network, NAS or remote server.

### SMB 2/3

Connect to compatible SMB network shares and browse music stored on your NAS, computer or home server.

### FTP

Connect to FTP servers and access your remote music collection.

**Security note:** Standard FTP does not encrypt its network traffic. Use it only on networks you trust.

### SFTP

Connect to compatible SFTP servers for music access over an encrypted SSH connection.

### Plex

Connect to your Plex Media Server and access your music library directly from DejiSa.

### Emby

Connect to your Emby Server and access your music library directly from DejiSa.

### Jellyfin

Connect to your own Jellyfin server to synchronize and stream your music library.

Local and network-based sources are brought together inside DejiSa instead of requiring a separate music player for each source.

---

## 📺 UPnP/DLNA playback

Enjoy your music beyond your phone.

DejiSa supports UPnP/DLNA output for compatible playback devices on your local network.

Features include:

- Discovery of compatible network playback devices
- Selection of available UPnP/DLNA renderers
- Playback through compatible network audio equipment
- Local-network permission handling on supported Android versions

Use your phone to choose the music and a compatible network device to play it.

UPnP/DLNA is an **audio-output feature**, not an additional music-library source.

Availability depends on your network configuration and the capabilities of your receiving device.

---

## ✨ Crystal Glass interface

DejiSa features a custom-designed interface with three visual themes.

### 🌕 Moonstone Crystal Glass

A light daytime appearance.

### 💜 Amethyst Crystal Glass

An atmospheric evening appearance.

### 🌑 Melanite Crystal Glass

A deep-night appearance with true AMOLED black.

Themes can switch automatically based on the local time or be selected manually.

### Additional interface features

- Custom 3D glyph controls
- Adaptive Crystal Dock
- Sensor-driven specular lighting
- Wallpaper and slideshow backgrounds
- Customizable dock positioning
- Adaptive layouts for phones, foldables and tablets
- Support for different screen sizes and orientations

The interface adapts to your device while retaining DejiSa's distinctive Crystal Glass design.

---

## DejiSa Surreality audio engine

DejiSa includes its own audio-processing engine: **DejiSa Surreality**.

Surreality is built around a high-precision audio pipeline with **64-bit DSP calculations** and adaptive output handling for Android devices, headphones, speakers and external DACs.

Audio features include:

- 64-bit digital signal processing
- Adaptive Hi-Res PCM output
- 32-bit float output on supported Android audio routes
- Automatic safe output fallback when a requested format is unavailable
- Surreality DSP and Surreality Pure playback modes
- 10-band graphic equalizer
- Parametric EQ
- Automatic DSP headroom management
- ReplayGain support
- Adaptive normalization
- Peak protection and limiting
- Spatial audio processing
- Personal audio calibration
- Per-device audio profiles
- Device-specific sound optimization
- Multichannel downmix support
- Direct DAC audio functionality
- USB audio device detection and diagnostics
- Configurable playback cache
- Live audio route and format inspection

### Surreality DSP

**Surreality DSP** processes decoded PCM audio using 64-bit calculations before sending it to the Android audio output.

Depending on the active audio route, Surreality can automatically select an appropriate output format. For example, a 16-bit / 44.1 kHz FLAC source can remain at its native sample rate while the DSP pipeline outputs 32-bit float PCM when supported.

The additional output precision does not recreate information that is absent from the original recording. Instead, it provides additional numerical headroom for DSP processing, mixing, equalization and volume calculations before final playback.

### Surreality Pure

**Surreality Pure** bypasses the Surreality DSP processing stages for users who want an unprocessed playback path.

Android, Media3, Bluetooth hardware or connected DACs may still perform their own conversion, mixing or resampling, so Pure mode by itself does not imply bit-perfect playback.

### Adaptive output

Surreality can inspect and adapt to the available Android audio route instead of blindly forcing an unsupported format.

Supported routes may use formats such as:

- 16-bit PCM
- 24-bit PCM
- 32-bit PCM
- 32-bit float PCM

When a selected format is unavailable, Surreality safely falls back to a compatible output instead of breaking playback.

**Note:** Available audio-processing features, output precision, Direct DAC functionality and supported audio routes depend on the Android device, operating system, connected hardware and audio driver capabilities.

---

## 📡 Plex, Emby & Jellyfin integration

DejiSa can connect to multiple media-server ecosystems while keeping playback and browsing inside one application.

### Plex

Connect DejiSa to your Plex Media Server and bring your Plex music collection into DejiSa alongside your other configured sources.

### Emby

Connect DejiSa to your Emby Server and bring your Emby music collection into DejiSa alongside your other configured sources.

### Jellyfin

Connect DejiSa to your self-hosted Jellyfin server.

Supported Jellyfin features include:

- Music library synchronization
- Artist, album and track browsing
- Playlist access
- Offline album downloads
- Configurable synchronization
- Quick Connect support
- Background synchronization
- Cache and library management

Your Plex, Emby and Jellyfin collections can become part of DejiSa's unified music experience.

**Media-server integration is optional.** DejiSa can also operate using local music and other configured sources.

---

## 📻 Internet radio

Discover and organize radio stations from around the world.

Features include:

- Browse stations by continent and country
- Customize available countries
- Save your favorite stations
- Access favorites directly from Home
- Dedicated radio playback interface

Explore international radio without leaving your music player.

---

## 📱 Home-screen widgets

DejiSa includes five resizable Android home-screen widgets.

1. Compact Player + Recognize
2. Compact Player
3. Large Player
4. Seek Player
5. Recognize-only

Widgets support:

- Adaptive layouts
- Horizontal and vertical resizing
- Optional transparent backgrounds
- Playback controls where applicable
- Music recognition shortcuts

Control your music or start recognition directly from your Android home screen.

---

## 🔎 Music recognition with Vigilsoni

DejiSa can connect to a compatible Vigilsoni service for additional music discovery functionality.

Supported integration includes:

- Music recognition
- Recognition history
- Short audio-sample recognition
- Artist following
- New release notifications
- Concert notifications

Connection is established through QR-code pairing.

When you start music recognition, DejiSa records a short audio sample and sends it to the configured Vigilsoni service through an authenticated ntfy relay.

Vigilsoni processes the recognition request and sends the result back to DejiSa through UnifiedPush.

Recognition history and artist-following features are also integrated into the application.

**Vigilsoni requires a compatible service and configuration.**

---

## 🔔 Notifications with ntfy & UnifiedPush

DejiSa integrates with **[ntfy](https://ntfy.sh/)** and **[UnifiedPush](https://unifiedpush.org/)** for notifications and communication with Vigilsoni.

Supported functionality includes:

- New music release notifications
- Concert notifications
- Music recognition results
- Artist-following responses
- Recognition-related events

### How it works

**Outgoing requests**

DejiSa sends supported requests, including short music-recognition audio samples, to Vigilsoni through an authenticated ntfy relay.

**Incoming notifications**

Vigilsoni delivers supported events and recognition results back to DejiSa through UnifiedPush.

**Your choice of distributor**

Use ntfy as your UnifiedPush distributor or choose another compatible distributor.

You can also use your own compatible ntfy server.

This architecture avoids requiring Google Firebase Cloud Messaging for DejiSa's Vigilsoni notifications and gives users more control over notification delivery.

---

## 💾 Offline music and playlists

Take your music with you.

DejiSa supports offline listening through downloaded music and local files.

Features include:

- Offline album downloads
- Offline music browsing
- Locally managed playlists
- Playlists containing tracks from different music sources
- Playback cache with configurable storage limits
- Application-wide Offline Mode

DejiSa playlists are independent of Plex, Emby and Jellyfin accounts.

An application-wide Offline Mode keeps local and downloaded music available while pausing remote services.

Your downloaded music remains accessible when your music server or internet connection is unavailable.

---

## 🎶 Playback features

DejiSa provides a full music playback experience through Android's Media3 playback framework.

Features include:

- Background audio playback
- Playback queues
- Shuffle and repeat
- Interactive seeking
- Lyrics
- Album artwork
- Playlist management
- Audio-output selection
- Configurable playback caching
- Headset and media-control integration

Browse your collection, manage your queue and control playback from within DejiSa or supported Android media controls.

---

## 🔄 Backup and restore

Back up your application settings and music configuration.

Supported options include:

- Local `.dejisa` backup files
- WebDAV backup storage
- Optional inclusion of credentials
- Optional password-protected encryption
- Playlist restoration
- Settings restoration

Choose local storage or a configured WebDAV destination.

**Keep your backups and recovery passwords somewhere safe.**

---

## 🔐 Privacy and security

DejiSa is designed with privacy in mind.

The application is developed without:

- Advertising SDKs
- Analytics SDKs
- Behavioral telemetry

Additional privacy features include:

- Android Keystore-backed credential protection where applicable
- Optional encrypted backups
- Local-first playlist storage
- Local profiles with optional biometric authentication
- Configurable music and network sources
- Optional self-hosted services
- UnifiedPush-based Vigilsoni notifications

Network access is used only where required for configured functionality, such as:

- Plex
- Emby
- Jellyfin
- Internet radio
- Remote music sources
- Artwork and metadata retrieval
- Vigilsoni
- ntfy and UnifiedPush

Local music playback does not require Plex, Emby, Jellyfin or another media-server account.

---

## 📦 Installation

1. Open the latest release.
2. Expand **Assets**.
3. Download the DejiSa APK.
4. Open the APK on your Android device.
5. Allow installation from the selected source if Android requests permission.
6. Install and launch DejiSa.

For updates, download the latest signed APK and install it over your existing installation.

---

## 🔄 Updates and releases

All official DejiSa APK releases are published through GitHub Releases.

**[⬇ Download the latest release](https://github.com/bigtechstruggler/DejiSa-Downloads/releases/latest)**

**[📦 View all releases](https://github.com/bigtechstruggler/DejiSa-Downloads/releases)**

This repository provides public application information and documentation.

APK distribution takes place through the linked release repository.

The full Android application source is maintained separately and is not included in the public distribution repository.

Automatically generated GitHub source archives contain the files present in the corresponding public release repository, not the separately maintained private application source.

---

## ❤️ A very special thank-you

A huge thank-you to **[Philipp C. Heckel](https://github.com/binwiederhier)**, the creator of ntfy, everyone who contributes to the project, and the people behind UnifiedPush.

You've made something genuinely useful, beautifully simple, and wonderfully independent.

**After the wheel and fire, ntfy might just be humanity's next great invention.** 🔥🛞🔔

Seriously, thank you for making this possible.

---

## 🇯🇵 About the name

DejiSa is derived from the Japanese expression for digital sound:

**デジタルサウンド — *Dejitaru Saundo***

Deji + Sa.

---
## ❤️ Support this project

If you enjoy this project and want to support my work:

[☕ Support me on Ko-fi](https://ko-fi.com/bigtechstruggler)

Your support helps me keep building and maintaining my projects — and gets me one tiny step closer to that Jaguar XJ8 (X350). 🐆

Support is completely optional. The software remains free.
# DejiSa — Your music. Your sources. Your sound. 🎵
