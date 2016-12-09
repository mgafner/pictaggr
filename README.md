# pictaggr
set exif tags in your pictures based on file and directory names

## About
given a directory of jpeg pictures:
```
~/Pictures/20160613_Ferien_Antalya_Public
```

your pictures in that directory will get these exif tags:
```
20160613
Ferien
Antalya
Public
```

pictaggr exif tags will be compatible to [shotwell](https://wiki.gnome.org/Apps/Shotwell/) exif tags

[shotwell](https://wiki.gnome.org/Apps/Shotwell/) is writing such tags in the *Keyword* exif tag:
```
mgafner@puzzle:~/$ exiftool -Keywords ~/Pictures/184631.jpg
Keywords                        : 20160613, Ferien, Antalya, Public
```

To write the tag as we want:
```
mgafner@puzzle:~/$ exiftool -Keywords="20160613, Ferien, Antalya, Public" ~/Pictures/184631.jpg
    1 image files updated
```


## Installation
#### Prerequisites
   * exiftool

#### Debian / Ubuntu
```
sudo apt-get install exiftool
```

## Usage
```
./pictaggr <target-directory>
```

## Useful links
   * exiftool: http://owl.phy.queensu.ca/~phil/exiftool/
   * shotwell: https://wiki.gnome.org/Apps/Shotwell/

## License
pictaggr is free software, available under the [GNU General Public License, Version 3](http://www.gnu.org/licenses/gpl.html).
