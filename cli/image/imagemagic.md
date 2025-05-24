## convert

### -border

```sh
magick convert $1 -bordercolor #000 -border 1 _brd_.png
```

### -crop

```sh
magick convert $1 -crop x1500 _%d_.png
```

### -paint

```sh
magick convert $1 -paint 3 $2
```

### -resize

```sh
magick convert $1 -resize x1600 -quality 100 _.jpg
```

### to pdf

```sh
magick convert "*.{png,jpeg}" -quality 100 _.pdf
```

## mogrify

### bmp to png

```sh
magick mogrify -format png $1
```

## montage

### -tile 1x

```sh
magick montage $1 -resize 750x -geometry +0+0 -tile 1x _montage_.png
```
