project(
    'singularity-desktop-session',
    version: '0.1.0.0',
    meson_version: '>= 1.10.0',
)

install_data(
    'src/singularity-start',
    'src/singularity-session',
    install_dir: get_option('bindir'),
    install_mode: 'rwxr-xr-x',
)

install_data(
    'data/singularity.desktop',
    install_dir: get_option('datadir') / 'wayland-sessions',
)

install_data(
    'config/labwc/rc.xml',
    'config/labwc/themerc',
    install_dir: get_option('datadir') / 'singularity' / 'labwc',
)

install_data(
    'data/icons/hicolor/scalable/apps/emblem-singularity.svg',
    'data/icons/hicolor/scalable/apps/dev.sinty.workspaces.svg',
    install_dir: get_option('datadir') / 'icons' / 'hicolor' / 'scalable' / 'apps',
)

install_subdir(
    'Singularity',
    install_dir: get_option('datadir') / 'icons',
    strip_directory: false,
)

install_data(
    'services/singularity-polkit-agent.service',
    'services/singularity-session.target',
    'services/xdg-desktop-portal-singularity.service',
    install_dir: get_option('prefix') / 'lib' / 'systemd' / 'user',
)

install_data(
    'data/portals/singularity.portal',
    install_dir: get_option('datadir') / 'xdg-desktop-portal' / 'portals',
)

install_data(
    'data/accountsservice/com.singularity.Desktop.xml',
    install_dir: get_option('datadir') / 'accountsservice' / 'interfaces',
)

install_data(
    'data/gschemas/dev.sinty.desktop.gschema.xml',
    install_dir: get_option('datadir') / 'glib-2.0' / 'schemas',
)
