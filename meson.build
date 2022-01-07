project('ncurses-vala-meson-demos', 'vala', 'c',
  version: '0.0.1')

add_project_arguments(['--enable-experimental'], language: 'vala')

vapi_dir = meson.current_source_dir() / 'vapi'

add_project_arguments(['--vapidir', vapi_dir], language: 'vala')

dependencies = [
  dependency('glib-2.0'),
  dependency('gobject-2.0'),
  meson.get_compiler('vala').find_library('posix'),
  meson.get_compiler('c').find_library('menu'),
  meson.get_compiler('c').find_library('curses'),
  meson.get_compiler('c').find_library('panel'),
  meson.get_compiler('vala').find_library('curses-fixes', dirs: vapi_dir),
  meson.get_compiler('vala').find_library('curses-panel', dirs: vapi_dir),
  meson.get_compiler('vala').find_library('curses-menu', dirs: vapi_dir),
]

subdir('src')
