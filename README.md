# arch-ISO
An ISO image I made based on an Arch Linux distro.

For now its just a simple arch installation ISO.

I will add a DE and more usefull stuff later.

## Building the image

You're going to need pacman as a packet manager in order to build the image.

Also install the package called archiso to build the image.
```bash
pacman -S archiso
```

Create a new directory and git clone the releng profile on it.
```bash
mkdir ~/iso
# Also create a directory called output in it
mkdir ~/iso/output
```


Open a terminal on the parent directory of releng and use this command 
```bash
mkarchiso -v -w /path/to/iso/dir/output -o /path/to/iso/dir/output /path/to/releng/
```

You might need to run this command with root access, just add "sudo" at the start.

And voilà, the iso image is located on 
```bash
~/iso/output/fluffyarch-2024.06.03-x86_64.iso
```

## TODO

- Add KDE plasma because why not
- Add system rescue tools
- Add calamares when KDE plasma is fully operational
- Maybe add a tiling Wayland compositor because i love hyprland and sway
- And other useful stuff when i have the time
