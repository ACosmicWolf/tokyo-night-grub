# Tokyo-Night for [GRUB](https://gnu.org/software/grub/)

> A dark theme for [GRUB](https://gnu.org/software/grub/).
Basically just minor tweaks of Dracula grub that I made to go along with my
[arch i3 rice](https://github.com/mino29/arch-i3).

![Screenshot](./screenshot.png)

This should fit all kinds of resolustion of screens, at least my 1080p screen
worked just fine.

## Install

Steps:

1. clone this repo or download the .zip

```bash
git clone https://github.com/mino29/tokyo-night-grub.git
```

2. copy the whole tokyo-night directory grub themes

```bash
sudo cp -r tokyo-night /boot/grub/themes
```

3. edit grub file

```
sudo vim /etc/default/grub
```
change `#GRUB_THEME=` to
`GRUB_THEME = "/boot/grub/themes/dracula/theme.txt"`

4.use magic and reboot

run this command
```
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

## Potential problems and solutions

Oh oh, can't see grub menu or boot into arch linux?

Grub on Arch Linux can be a pain to deal with recently.
After I change the theme and reboot and cannot boot into my Arch Linux, had to
do a "chroot", but worry not, here's what you need:

- USB drive with arch iso
- 15 minutes of free time
- Stable internet connection
- this on-point [article]()


## Credit

[Cute Ghost profile]()
[Dracula Grub]()

## License

[MIT License](./LICENSE)