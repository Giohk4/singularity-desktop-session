# Singularity-desktop-session

Unofficial package for the singularity desktop enviroment session.

## why ?

This package was made because packaging the official [singularity-desktop](https://github.com/singularityos-lab/singularity-desktop) and [singularity-session](https://github.com/singularityos-lab/singularity-session) were simply way too annoying to package, so i decided to make my own version of both as one thing adapted for packaging conventions.

### Note :
While this is made for the [Sinty RPMs Project](https://copr.fedorainfracloud.org/coprs/giohk404/Sinty/) it can be used as starting point to help you package it for other distributions, most of what's in here is compatible with most* modern distributions.

though, you should take a look around as i may have hard coded some RPM distro specific assumptions


## logging

if you want to check logs use

``journalctl -t <object>``  or use  ``journalctl -t <object> -f`` to track logs live.

replace <object> with one of the following

+ ``labwc`` => for labwc logs

+ ``singularity-session`` => logs of the session.

or alternativly you can use the gnome-logs app for a GUI way to do it.

## License

GPL-3.0 - see [LICENSE](LICENSE).
