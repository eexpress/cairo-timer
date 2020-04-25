icon_size = ['16', '32', '48', '64', '128']

foreach i : icon_size
    install_data(
        'cairo-timer_' + i + '.png',
        rename: meson.project_name() + '.png',
        install_dir: join_paths(get_option('datadir'), 'icons', 'hicolor', i + 'x' + i, 'apps')
    )
endforeach

install_data(
    meson.project_name() + '.desktop',
    install_dir: join_paths(get_option('datadir'), 'applications')
)

install_data(
    meson.project_name() + '.appdata.xml',
    install_dir: join_paths(get_option('datadir'), 'metainfo')
)

install_data(
    meson.project_name() + '.png',
    install_dir: join_paths(get_option('datadir'), 'pixmaps')
)
