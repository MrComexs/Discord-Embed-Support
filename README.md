# Discord-Embed-Support
PC = Windows 10 / Arch Linux
- Discord app
- Vesktop
- Vencord

Mobile = Android 14 One UI 6.1

# Audio playback support
tool: `flac` `ffmpeg` `lame` 

note: for ACC its AAC_LC and it was from a random file I had. I wasn't able to use ffmpeg to make a acc file.

WAV 64 bit float point isn't supported.
| Container | PC  | Mobile |
| --------- | :-: | :----: |
| mka       |  ✘  |   ✘    |

| Codec  | Container | PC? | Mobile | Encoder   |
| ------ | --------- | :-: | :----: | --------- |
| ACC    | m4a       |  ✔  |   ✘    |           |
| ACC    | mka       |  ✘  |   ✘    |           |
| FLAC   | flac      |  ✔  |   ✘    | libflac   |
| MP3    | mp3       |  ✔  |   ✘    | lame      |
| OPUS   | ogg,opus  |  ✔  |   ✘    | libopus   |
| Vorbus | ogg       |  ✔  |   ✘    | libvorbis |
| WAV    | wav       |  ✔  |   ✘    | ffmpeg    |

# Image preview support 
tool: `imagemagick`

I think imagemagick uses libheif for avif.
| Codec | PC  | Mobile | Encoder        |
| ----- | :-: | :----: | -------------- |
| avif  |  ✘  |   ✘    | libheif?       |
| heif  |  ✘  |   ✘    | libheif        |
| jpg   |  ✔  |   ✔    | libjpeg-turbo |
| jxl   |  ✘  |   ✘    | libjxl         |
| png   |  ✔  |   ✔    | libpng         |
| webp  |  ✔  |   ✔    | libwebp        |

# Animation preview support
tool: `ffmpeg`
| Codec | PC  | Mobile |
| ----- | :-: | :----: |
| avif  |  ✘  |   ✘    |
| gif   |  ✔  |   ✔    |
| jxl   |  ✘  |   ✘    |
| png   |  ✘  |   ✘    |
| webp  |  ✔  |   ✔    |

# Video playback support
tool:`ffmpeg`

`h265` On my Arch Linux install the first frame is the only frame but the audio doesn't have any issues.
| Container | PC  | Mobile |
| --------- | :-: | :----: |
| mkv       |  ✘  |   ✘    |
| mov       |  ✔  |   ✔    |
| mp4       |  ✔  |   ✔    |
| webm      |  ✔  |   ✔    |

| Codec | PC  | Mobile | Encoder    |
| ----- | :-: | :----: | ---------- |
| av1   |  ✘  |   ✘    | libsvtav1  |
| h264  |  ✔  |   ✔    | libx264    |
| h265  |  ✔  |   ✔    | libx265    |
| vp9   |  ✔  |   ✔    | libvpx-vp9 |

| Codec  | PC? | Mobile | Encoder    |
| ------ | :-: | :----: | ---------- |
| ACC    |  ✔  |   ✔    |            |
| FLAC   |  ✔  |   ✔    | libflac    |
| MP3    |  ✔  |   ✔    | libmp3lame |
| OPUS   |  ✔  |   ✔    | libopus    |
| Vorbus |  ✔  |   ✘    | libvorbis  |
| WAV    |  ✔  |   ✘    | ffmpeg     |

---
# Licenses
CC BY-SA-4.0
