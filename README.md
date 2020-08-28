# Main Laboratory of ZX Basic

Main Laboratory of ZX Basic

## 1. Operating System used

We are using Ubuntu 20.04.01 Budgie when writing this mini guide.

## 2. FUSE Installation

FUSE is the ZX-Spectrum Emulator that we are going to use for Linux.

There are two versions available:

- Fuse (SDL): SDL (Simple DirectMedia Layer) 
- Fuse (GTK+)

We choose the __GTK+__ and install it from the software center.

When starting FUSE, it will indicate that it has not found the ZX-Spectrum ROMs.

To install the roms, we have to do:

```shell
$ sudo apt-get install spectrum-roms fuse-emulator-utils
```

With this, when starting FUSE, the system should already recognize the ROMs.

## 3. zxb compiler Installation

Get the zxb compiler from this url:

```url
https://www.boriel.com/files/zxb/
```

Extract the archives and copy to our home user directory, for example in /home/<user>/Programs/zxbasic

## 5. Setting environment variables

We add the following to the .profile file:

```
#zxb
export PATH=${PATH}:${HOME}/Programs/zxbasic
```

We leave and re-enter the session

It is done.

After this, you could try the Helloworld example.

Enjoy it!