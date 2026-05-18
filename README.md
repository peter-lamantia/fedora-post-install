# Fedora Post-install
All the things I add/change/install to make Fedora work better for me.

This is based on a Fedora 44 install at the time of writing.

## Setup 

### Add RPMFusion repositories

Quote: "RPM Fusion provides software that the Fedora Project or Red Hat doesn't want to ship."

Follow [this guide](https://rpmfusion.org/Configuration) for setup.


### Add better codec support

Fedora does not ship with some codecs out of the box due to licensing reasons. Assuming you already have RPMFusion set up from earlier, [let's fix that](https://rpmfusion.org/Howto/Multimedia)!


### Gnome Extensions

This is more personal preference, but I use a couple extensions to make Gnome more pleasant to use. 

First, you need to install the [Extensions app](https://apps.gnome.org/Extensions/) or [Extension Manager](https://mattjakeman.com/apps/extension-manager) (even better).

A list of extensions can be found on [this site](https://extensions.gnome.org/). I like clicking the blue install button, but you can also download and install manually if you like.

Some of my favorite Gnome extensions:
- Caffeine: like Amphetamine from macOS, allows you to prevent the screen from sleeping for a set period of time or indefinitely.
- Hot Edge: allows you to trigger the multitask view by mousing to the bottom edge. Fantastic.
- Removable Drive Menu: it's in the name, see removable drives on the top bar.
- System Monitor: see all those juicy stats right on the top bar.


### Install the Nvidia drivers (if you have a Nvidia GPU)

...and silently curse Nvidia for not shipping an open driver like AMD. This has implications for secure boot because the driver is a kernel mod and appears untrusted. I'll explain more about this later.

Follow [this guide](https://rpmfusion.org/Howto/NVIDIA?highlight=%28%5CbCategoryHowto%5Cb%29) for instructions. Be sure to wait for the driver to fully build!


### Set up Secure Boot

More to come here. 


### Decrypt boot drive with TPM

I need to write more, but [here's a guide to that](https://fedoramagazine.org/automatically-decrypt-your-disk-using-tpm2/).


### Play some games

Honestly, Steam does a pretty good job here. But [GE-Proton](https://github.com/GloriousEggroll/proton-ge-custom) is also great to fix bleeding-edge issues and add performance. I don't use this unless the game does not launch correctly.


