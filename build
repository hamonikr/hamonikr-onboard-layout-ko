#!/bin/bash

PKG=`cat debian/DEBIAN/control | grep Package | cut -d' ' -f 2`
VER=`cat debian/DEBIAN/control | grep Version | cut -d' ' -f 2`

echo "Packaging Start... Please Wait a while..." 

echo "Generate md5 chucksum file" 
find debian/usr -type f -exec md5sum {} \; > debian/DEBIAN/md5sums
sed -i 's/debian\///g' debian/DEBIAN/md5sums

echo "Building debian package" 
dpkg-deb --build debian

if [ ! -d ./release ]; then
  mkdir release
fi

mv debian.deb release/${PKG}-${VER}_all.deb

echo "Use below command for Install"
echo "============================="
echo "sudo dpkg -i release/${PKG}-${VER}_all.deb" 
