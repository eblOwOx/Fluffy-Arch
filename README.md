# arch-ISO
An ISO image i made based on a Arch Linux distro.

For now its just a simple arch installation.

I will add a DE later.

# Building the image

You're gonna need pacman as a packet manager in order to build the image.

Use the package called archiso to build the image.

Create a new directory and git clone the releng profile on it.
Open a terminal on the parent directory of releng and use this command "mkarchiso -v -w ~/iso/output -o ~/iso/output /path/to/releng/" (you might need to run this command with root access, just add "sudo" at the start).

And voilà, the iso image is located on ~/iso/output
