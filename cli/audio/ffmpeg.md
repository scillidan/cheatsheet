## .m4b optimizate

```sh
ffmpeg -i $1 -map 0:a -map_metadata 0  -c:a aac -b:a 64k -id3v2_version 3 -movflags +faststart _opti_.m4b
```

## to mp3

### aac

```sh
ffmpeg -i $1 -codec:a libmp3lame -qscale:a 1 _aac2_.mp3
```

### m4a

```sh
ffmpeg -i $1 -c:a libmp3lame -q:a 8 _m4a2_.mp3
```

```sh
ffmpeg -i $1 -vn -c:a libmp3lame -b:a 224K -ac 2 _m4a2_.mp3
```

### video

```sh
ffmpeg -i $1 -map 0:a:0 -c:a copy _vid2_.mp3
```

## to ogg

### audio

```sh
ffmpeg -i $1 -map_metadata -1 -c:a libvorbis -b:a 64k -compression_level 10 -vn _aud2_.ogg
```

```sh
# for voice recording
ffmpeg -i $1 -c:a libvorbis -ar 44100 -b:a 128k -maxrate 192k -minrate 64k -bufsize 192k _aud2_.ogg
```

```sh
# for music
ffmpeg -i $1 -c:a libvorbis -ar 44100 -b:a 256k -maxrate 320k -minrate 128k -bufsize 320k _aud2_.ogg
```
