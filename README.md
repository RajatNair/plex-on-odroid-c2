# Plex Media Server on Odroid C2 running Ubuntu arm64 (based on plexmediaserver-installer repo)

## Dependency
sudo apt-get install fakeroot

## Build
1. Create a working copy: 
`bash
mkdir ../plex-installer; git archive master | tar -x -C ../plex-installer/
`
2. Build the package: 
`bash
cd ..; fakeroot dpkg-deb --build plex-installer ./
`

## Version (ARM 6.x RN2xx)
PMS version - 1.12.0.4829-6de959918
Date - February 27, 2018
SHA-1 Checksum - 4f9b07b8c52cda1b34e0c6d9d3fa60a4fa99e548
