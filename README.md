# bash-toolbox
A collection of handy bash scripts that I use from time to time.

## yt-dlp_mp4
Uses yt-dlp as a downloader backend, with additional flags for higher audio quality when converting to mp4 via ffmpeg (named 'VideoConvertor' in yt-dlp).
If yt-dlp is not already present it can be installed with:
```bash
python3 -m pip install -U yt-dlp
```
Usage:
```bash
yt-dlp_mp4 <Video URL>
```
