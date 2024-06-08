# Fluffy Arch
A distro made for my own pleasure.

For now its just a simple Arch Linux distro with KDE plasma.

But guess what? I broke everything... cool (okay i just forgot to add the sddm symlink woops)

I'll also customize the look and add more useful things later.

## Specificity
This distro was made for x86-64 arch processor.

Works with and without UEFI.

Still under developpment, expect bugs or stuff breaking.

## Building the image

There's maybe others ways to do it, but for now its the only way i found to build the image.

You're going to need pacman as a packet manager in order to build the image.

Also install the package called archiso to build the image.
```bash
pacman -S archiso
```

Create a new directory and git clone the releng profile on it.
```bash
mkdir ~/iso
git clone https://github.com/eblOwOx/arch-ISO.git
```


Open a terminal on the parent directory of releng and use this command 
```bash
mkarchiso -v -w output/ -o output/ releng/
```

You might need to run this command with root access, just add "sudo" at the start.

And voilà, the iso image is located on 
```bash
~/iso/output/fluffyarch-yyyy.mm.dd-x86_64.iso
```

## TODO

- Add KDE plasma because why not (DONE)
- Customize KDE plasma and sddm
- Switching to grub instead of systemd-boot
- Add more system rescue tools
- Add calamares when KDE plasma is fully operational
- Maybe add a tiling Wayland compositor because i love hyprland and sway
- And other useful stuff when i have the time
- Also make the distro bootable with a mutli-boot utility like ventoy because it doesn't work
