### curl,sd,mdtable2csv,xsv,csview

```sh
curl -k https://raw.githubusercontent.com/scillidan/WALLPAP-ENG-resource/main/table.md | sd "\[\d{10}\]\(" "" | sd "(\)\|\S+subsc)" "|![](//img.shields.io/steam/subsc" | mdtable2csv | sd "//steamc" "https://steamc" | xsv select source,version,urlid | csview
```

### curl,mdtable2csv,xsv,tidy-viewer,coloro,less

```sh
curl -k --remote-name-all -o - https://raw.githubusercontent.com/scillidan/color/main/data/{chinese-traditional-colors.md,china-tradition-color-monokuro.md,zhongguose.md,china-tradition-color-320.md,nipponcolors.md} | mdtable2csv | xsv select hex,spelling,name | tidy-viewer -D -a -e | coloro | less -R
```

### linkding-cli,jq,ramda-cli,xsv,tidy-viewer

```sh
linkding --url "http://127.0.0.1:8002" --token "<token>" bookmarks all -q $1 | jq ".results[]" | ramda -c -o csv | xsv select tag_names,url,website_title | tidy-viewer -u 45
```