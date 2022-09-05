# bash-toolbox
A collection of handy bash scripts that I use from time to time.

### Linux
If yt-dlp is not currently installed it can be installed with:
```bash
python3 -m pip install -U yt-dlp
```
FFmpeg is required for yt-dlp to work properly and can be installed using:
```bash
sudo apt install ffmpeg -y
```
### macOS
If you are running macOS, both yt-dlp and ffmpeg can be installed using brew:
```
brew install yt-dlp ffmpeg
```

## yt-dlp_mp3
Uses yt-dlp to download audio stream only, then converts to a 320kbps MP3 file.

#### Usage:
```bash
./yt-dlp_mp3 <URL1> <URL2> ...
```

## yt-dlp_mp4
Uses yt-dlp as a downloader backend, with additional flags for higher audio quality when converting to mp4 via ffmpeg (named 'VideoConvertor' in yt-dlp).

#### Usage:
```bash
./yt-dlp_mp4 <URL1> <URL2> ...
```

## yt-dlp_discord
Downloads video/audio using yt-dlp while also converting the input to a desired filesize (under 8MB default). Flag `-n` (Nitro Classic) can be passed to increase target size to 40MB. Flag `-a` fetches audio stream only and converts the output to MP3 with dynamic bitrate based on desired output filesize. Flag `-v` enables verbose mode.

#### Usage:
```bash
./yt-dlp_discord [OPTIONS] <URL1> <URL2> ...
```

## yt-dlp_quickview
Downloads video to tmp using yt-dlp and automatically opens it in a media player. Deletes the file automatically when media player is closed. Paths and variables may be changed before running.

#### Usage:
```bash
./yt-dlp_quickview <URL>
```

## sha256check
Verifies SHA-256 checksums of files using `sha256sum`. Allows the user to specify a different checksum file if needed.

#### Usage:
```bash
./sha256check <FILE>
```
