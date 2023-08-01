# MOTIVATION scan from EPSON multi printer/scanner inside bash

## install used software packages cli bash

````bash
sudo apt install sane sane-utils ```

## find scanner

```bash
scanimage -L
````

## test scan to file ( during a while)

```bash
scanimage --resolution 300 --mode color > /tmp/test-epson.ppm
```

## test scan with format png

```bash
scanimage --resolution 300 --mode color --format png > /tmp/test-epson.png
```

## test scan with scanner name to file

```bash
scanimage -d 'airscan:w1:EPSON ET-3750 Series' --resolution 300 --mode color --format png > /tmp/test-epson_with_sanner_name.png
```
