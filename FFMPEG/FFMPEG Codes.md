# FFMPEG

## //Convert .MKV to .MP4
_ffmpeg -i xXxX.mkv -codec copy xXxX.mp4_

## //Convert .OGG to .MP3
_ffmpeg -i xXxX.OGG -acodec libmp3lame xXxX.mp3_

## //Extract especific audio track
_ffprobe //see all audio tracks of a file_
_ffmpeg -i xXxX.ext -map "#1":"#2" xXxX.ext_

## //Low audio bit
_ffmpeg -i input.file -map 0:*a*:0 -b:a 96k output.mp3_
