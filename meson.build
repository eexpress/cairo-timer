
project('com.github.eexpress.cairo-timer', 'vala', 'c')

# i18n = import('i18n')
# add_global_arguments('-DGETTEXT_PACKAGE="@0@"'.format (meson.project_name()), language:'c')

executable(
	meson.project_name(),
	'src/Application.vala',
	dependencies: [
		dependency('gtk+-3.0')
	],
#	link_args : '-X',
#	link_args : '-lm',
	link_args : ['-X', '-lm',],
	install: true
)

install_data(
	join_paths('data', meson.project_name() + '.desktop'),
	install_dir: join_paths(get_option('datadir'), 'applications')
)

install_data(
	join_paths('data', meson.project_name() + '.appdata.xml'),
	install_dir: join_paths(get_option('datadir'), 'metainfo')
)

