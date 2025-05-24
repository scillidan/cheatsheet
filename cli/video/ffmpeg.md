## export poster

### -vframes

```sh
ffmpeg -i $1.mp4 -vframes 1 _poster_.jpg
```

## export subtilte

### srt

```sh
ffmpeg -i $1 -map 0:s:0 _sub_.srt
```

### sup

```sh
ffmpeg -i $1 -map 0:s:0 -c:s copy _sub_.sup
```

## to mp4

### gif

```sh
ffmpeg -i $1.gif -movflags faststart -pix_fmt yuv420p -vf "scale=trunc(iw/2)*2:trunc(ih/2)*2" _gif2_.mp4
```

### image

```sh
ffmpeg -framerate 1 -i $04d.png -c:v libx264 -r 30 -pix_fmt yuv420p _img2_.mp4
```

```sh
ffmpeg -framerate 30 -i $04d.png -c:v libx264 -pix_fmt yuv420p _img2_.mp4
```

```sh
ffmpeg -loop 1 -i $1 -vf "scale=trunc(iw/2)*2:trunc(ih/2)*2" -c:v libx264 -t 1 -pix_fmt yuv420p _img2.mp4
```

### video

```sh
ffmpeg -i $1 -map 0 -c:v copy -c:a ac3 -b:a 256K -ac 2 -c:s copy _vid2_.mp4
```