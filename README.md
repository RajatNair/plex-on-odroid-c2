# Plex Media Server on Odroid C2 running Ubuntu arm64 (based on plexmediaserver-installer repo)

## Dependency
```bash
sudo apt-get install fakeroot
```

## Build
```bash
mkdir ../plex-installer; git archive master | tar -x -C ../plex-installer/ && cd .. && fakeroot dpkg-deb --build plex-installer ./
```

## Install
```bash
sudo dpkg -i /path/to/deb/file && sudo apt-get install -f
```

## Version (ARM 6.x RN2xx)
PMS version - 1.12.0.4829-6de959918

Date - February 27, 2018

SHA-1 Checksum - 4f9b07b8c52cda1b34e0c6d9d3fa60a4fa99e548
