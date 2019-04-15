## Introduction
Change the way you look at your desktop. Get carefully crafted, bright and clean icon-theme for
Linux.


- [Installation](#installation)
- [Whats New](#whats-new)
- [New Icon Request](#new-icon-request)
- [Troubleshoot](#troubleshoot)
  - [Icon themed but does not appear](#icon-themed-but-does-not-appear)
- [Coffee and Cookies](#coffee-and-cookies)
- [My Other Apps](#my-other-apps)




*Dual* is a flat icon-theme for gnome 3.20+. The icons have colourful circular base with dual tone.

As of version 1, it contains 1100+ apps icon , 2200+ icons in total and counting.

## Installation

Installation in straight forward.
> From [Github](https://github.com/rudrab/dual):
* If you are not using `dual` already:<br>
    `mkdir -p ~/.icons`<br>
    `cd ~/.icons`<br>
    `git clone https://github.com/rudrab/dual.git`
* From the next time:
    `cd ~/.icons/dual`<br>
    `git pull`


> Download from [gnome-look.org](https://www.opendesktop.org/p/1234339/)
*  `cd ~/.icons`<br>
   `mkdir -p dual`<br>
   `cd dual`<br>
   `tar -Jxvf <Your download path>/dual<version>.tar.xz`

Activate the theme using `tweak-tool` or from command line:
      
      gsettings set org.gnome.desktop.interface icon-theme "dual"


#### Optional: Icon themes

*Version 3* includes many new icons. Plus 5 gem themed *places* i.e. folder icons based on ruby,
emerald, garnet, sapphire(default) and torquise beside a oldish square icons. 

There is a python script named `changecolor.py` in the parent folder. Just run this as

    python3 changecolor.py

and choose your desktop environment and colour theme.

Hope you will like it.

## Whats New
**Version 1.0**
  > * Ready for gnome 3.32
  > * Current release contains around ~1200 app icons. 

## New Icon Request:
Don't hesitate to contact me if you want new icons to be themed.

Please [raise icon request issue here](https://github.com/rudrab/dual/issues). 
Don't forget to add  ***"Icon request"*** label. 

### How to request new icons

For faster creation of new files, kindly give me those information:
If you are requesting icon `foo`, kindly send me `foo.desktop` file or atleast the Icon line from
the file. If you have installed the package from your package manager, it should live on
`/usr/share/applications/foo.desktop`. If you have installed it yourself, most likely, it will be
either at `/usr/local/applications/foo.desktop` (if you have installed it with root) or 
`~/.local/share/applications/foo.desktop` (if you have installed it without root). 

Another very helpful thing will be providing me the default icon. You can just grab a screenshot
with the icon visible and send it to me. But this is completely optional.

I will try my best to theme the icons ASAP.

## Troubleshoot
#### Icon themed but does not appear
 Most of the time, this is because, the corresponding desktop file has full path in icon name.
 like, for some app named Foo, the corresponding `foo.desktop` file (e.g.
 `/usr/share/applications/foo.desktop`) may look like:
 ```
[Desktop Entry]
Name=Foo
Exec=foo
Icon=/usr/share/icons/hicolor/foo-icon.png
 ```

This can not be themed. The workaround is to copy it to your `~/.local/share/applications/`
and give the icon generic path like:
```
[Desktop Entry]
Name=Foo
Exec=foo
Icon=foo-icon
 ```

## Coffee and Cookies
If you like the theme, don't forget to upvote it at [gnome-look](https://www.opendesktop.org/p/1234339/).

If you _really_ like the theme, please buy me a coffee using [PayPal](https://www.paypal.me/banerjeerudra). 

## My Other Apps

See other apps I have developed:

- [MkBiB](http://rudrab.github.io/MkBiB/): BiBTeX Manager

- [Periodic Table](http://rudrab.github.io/PeriodicTable/): Periodic Table and Extra

- [Shadow](http://rudrab.github.io/Shadow/): Icon theme for Gnome desktop

- [dual](http://rudrab.github.io/dual/): Icon theme for Gnome desktop

- [vimf90](http://rudrab.github.io/vimf90/): Firtran plugin for vim
