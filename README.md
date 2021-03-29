### libnpupnp/upmpdcli Archlinux

> pacman -Sy aspell aspell-en id3lib jsoncpp python-appdirs python-bottle  python-chardet python-ordered-set  python-packaging python-setuptools  python-six  python-urllib3  python-waitress
>
> pacman -U libnpupnp-4.0.14-1-aarch64.pkg.tar.xz
>
> pacman -U libupnpp-0.19.4-1-aarch64.pkg.tar.xz
> 
> pacman -U upmpdcli-1.4.14-1-aarch64.pkg.tar.xz
>
> cp upmpdcli.conf /etc/upmpdcli.conf
>
> cp upmpdcli.service /lib/systemd/system/
> 
> systemctl daemon-reload
> 
> systemctl stop mpd.socket
>
> systemctl stop mpd

Enable port 6600  "/etc/mpd.conf"

> 
> systemctl enable upmpdcli
> 
> systemctl restart upmpdcli
>
> systemctl restart mpd
>
> systemctl restart mpd.socket
>
> systemctl status upmpdcli
> 
> systemctl status mpd


#### Cookbook by TuanQuynhAudio
