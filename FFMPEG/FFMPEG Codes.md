//Convert .MKV to .MP4
ffmpeg -i xXxX.mkv -codec copy xXxX.mp4

//Convert .OGG to .MP3
ffmpeg -i xXxX.OGG -acodec libmp3lame xXxX.mp3

//Extract especific audio track
ffprobe //see all audio tracks of a file
ffmpeg -i xXxX.ext -map "#1":"#2" xXxX.ext

//Low audio bit
ffmpeg -i input.file -map 0:a:0 -b:a 96k output.mp3