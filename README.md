## Numix Green
##### A modern flat theme with a combination of light and dark elements. It supports GNOME, Unity, Xfce and Openbox.

Numix Green is a fork of [Numix](https://github.com/numixproject/numix-gtk-theme) and is inspired in [other previous green theme](https://github.com/Yharooer/numix-green). Numix is a part of the [Numix Project](http://numixproject.org).

### Manual installation

First, you need to compile the theme using the [Sass](http://sass-lang.com/) compiler.

To install Sass, install Ruby and the gem command using your distribution's package manager. Then install `sass` with the `gem` command,

`gem install sass`

You'll also need the following commands in your path to generate the gresource binary. Install them using your distribution's package manager.

* `glib-compile-schemas`
* `gdk-pixbuf-pixdata`

After installing all the dependencies, switch to the cloned directory and, run the following in Terminal,

```sh
make
sudo make install
```

To set the theme in GNOME, run the following commands in Terminal,

```sh
gsettings set org.gnome.desktop.interface gtk-theme "Numix Green"
gsettings set org.gnome.desktop.wm.preferences theme "Numix Green"
```

To set the theme in Xfce, run the following commands in Terminal,

```sh
xfconf-query -c xsettings -p /Net/ThemeName -s "Numix Green"
xfconf-query -c xfwm4 -p /general/theme -s "Numix Green"
```

### Requirements

GTK+ 3.16 or above

Murrine theme engine

### Code and license

Report bugs or contribute at [GitHub](https://github.com/Madh93/numix-green-gtk-theme)

License: GPL-3.0+
