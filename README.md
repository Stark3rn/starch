# starch
setup guide for my custom arch linux version

## archinstall
the first step is to install arch linux. To do so, go to https://archlinux.org/download/ and download one of the links. Chose one hosted on your country to be faster.
You can do the install either on a virtual machine or a computer ssd/hdd.

### Keymaps
**/!\ It is a QWERTY keyboard by default. Be aware if you usually use AZERTY keyboard for instance.**
- to list keymaps, use `localectl list-keymaps`
- then to change the keymap, use `localectl set-keymap <keymap>`

### Internet/Wifi
If you are using ethernet connexion :
Verify internet connexion by using `ping archlinux.org`
It should work.

If you are using wifi connexion :
Configure your wifi connexion :
- `iwctl` - network configuration
- `station list` - list your PC's network stations
- `station <station> scan` - scans networks available
- `station <station> connect "wifiname" password` - connects to the wifi you want

### Installation guide

Now that you have wifi and the right keymap, you can run the installation guide by typing `archinstall`.
- For disk partition, do as you want, but i recommand to encrypt the disk with LVM using a long passphrase.
- Don't forget to add an audio manager, i'll use pipewire because it is more recent and modern but pulseaudio is okay too
- You can install packets with the installer's manager if you want to, but you will be able to do it later anyway.
- When finished, you can hit the "install" button.

## install starch

(complete later with .sh files)
