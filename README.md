# bash-toolbox
A collection of handy bash scripts that I use from time to time.

If yt-dlp is not currently installed it can be installed with:
```bash
python3 -m pip install -U yt-dlp
```
## yt-dlp_mp4
Uses yt-dlp as a downloader backend, with additional flags for higher audio quality when converting to mp4 via ffmpeg (named 'VideoConvertor' in yt-dlp).

Usage:
```bash
./yt-dlp_mp4 <Video URL>
```

## yt-dlp_quickview
Downloads video to tmp using yt-dlp and automatically opens it in a media player. Deletes the file automatically when media player is closed. Paths and variables may be changed before running.

Usage:
```bash
./yt_dlp_quickview <Video URL>
```
