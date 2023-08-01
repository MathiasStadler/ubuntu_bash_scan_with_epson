# MOTIVATION scan with/from EPSON ET-3750 Series multi printer/scanner inside bash

## install used software packages via cli bash

```bash
sudo apt install sane sane-utils
```

## find scanner via cli in the same network

```bash
scanimage -L
````

## test scan to file ( during a while)

```bash
scanimage --resolution 300 --mode color > /tmp/test-epson.ppm
```

## test scan with output format png

```bash
scanimage --resolution 300 --mode color --format png > /tmp/test-epson.png
```

## test scan with different scanner in the network

```bash
scanimage -d 'airscan:w1:EPSON ET-3750 Series' --resolution 300 --mode color --format png > /tmp/test-epson_with_sanner_name.png
```

sorry my english is so bad
