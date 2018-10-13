# Plex Media Server on Odroid C2 running Ubuntu arm64 (based on plexmediaserver-installer repo)

## Dependency
sudo apt-get install fakeroot

## Build
`bash
mkdir ../plex-installer; git archive master | tar -x -C ../plex-installer/ && cd .. && fakeroot dpkg-deb --build plex-installer ./
`

## Install
`bash
sudo dpkg -i /path/to/deb/file && sudo apt-get install -f
`

## Version (ARM 6.x RN2xx)
PMS version - 1.13.0.5003-8fcb5b6e5
Date - April 27, 2018
SHA-1 Checksum - 8dce11c15a2232a1abd7b790b3586725b7742c25
