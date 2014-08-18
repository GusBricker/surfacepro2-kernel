SURFACE PRO 2 LINUX KERNEL
==========================

This kernel has a few fixes for bluetooth and type/touch cover detection. It has only been tested on the Surface Pro 2.

## To Build

git clone https://github.com/GusBricker/surfacepro2-kernel.git
git checkout surfacepro2
sudo su
make-kpkg -j `getconf _NPROCESSORS_ONLN` --initrd --append-to-version=-surfacepro2 kernel_image kernel_headers kernel_source

## Manual Install

sudo dpkg -i linux-headers*.deb linux-image*.deb

## Scripted Install

I have written a nice setup script targetted at Ubuntu, go [here](https://github.com/GusBricker/surfacepro2-ubuntu-post-setup).
