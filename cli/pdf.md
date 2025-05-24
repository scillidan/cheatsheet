## analysis

### pdf_pdfalyzer.py

```sh
python pdf_pdfalyzer.py $1
```

## .dtx to pdf

### pdflatex

```sh
pdflatex --shell-escape $1
```

## .dvi to pdf

### dvipdfm

```sh
dvipdfm $1
```

## .html to epub

### paperoni

```sh
paperoni $1 --export epub
```

### percollate

```sh
percollate epub $1 -o _html2_.epub
```

## .html to pdf

### percollate

```sh
percollate pdf $1 -o _html2_.pdf --css ":root { --main-font: 'Beholden Medium';  --code-font: 'Beholden Medium'; --alt-font: 'Beholden Medium'; }"
```

## signature

### batchpdfsign

```sh
java -jar batchpdfsign-portable.jar -k <file.pfx> -p <password> -i $1 -o _sig_.pdf
```

### open-pdf-sign

```sh
java -jar open-pdf-sign.jar --input $1 --output _sig.pdf --certificate <file.crt> --key <file.pem> --passphrase <password> --page -1 --locale zh-CN
```

## toc

### pdf-toc

```sh
pdf-toc -t toc.txt -d _toc_.pdf $1
```

## watermark

```sh
markpdf $1 mark.png --opacity=0.3
```