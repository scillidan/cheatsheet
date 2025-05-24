### +matchpatch

```sh
gmic $1 $2 +matchpatch[0] [1],3 +warp[-2] [-1],0
```

### +srgb2lab,+blend

```sh
gmic $1 +srgb2lab slic[-1] 16 +blend shapeaverage f[-2] "j(1,0)==i && j(0,1)==i" *[-1] [-2]
```

### frame_xy
```sh
gmic $1 frame_xy 1,1,0 frame_xy 10,5,0,0,0
```

### grid

```sh
gmic $1 grid 10%,16%,0,0,0.2,255
```

### kuwahara

```sh
gmic $1 kuwahara 9
```

### montage

```sh
gmic $1 montage H1:V0:VH2:1H0:3
```

### quantize,blur

```sh
gmic $1 quantize 6 blur 1 round[-1] quantize_area[-1] 2
```

### quantize,+split_colors

```sh
gmic $1 quantize 3 +split_colors , display_rgba
```

### segment_watershed

```sh
gmic $1 segment_watershed 4
```

### topographic_map

```sh
gmic $1 topographic_map 10
```

