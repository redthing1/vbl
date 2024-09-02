project(
  'vbl',
  'cpp',
  license: 'GPL-2.0-or-later',
  default_options: ['cpp_std=c++11', 'buildtype=debugoptimized'],
  version: run_command('version.sh', check: false).stdout(),
)

ncurses_sh = [dependency('ncursesw')]
# ncurses_st = [dependency('ncursesw', static: true)]

vbl_sources = [
  './vbl.cpp',
]

vbl_exe = executable(
  'vbl',
  vbl_sources,
  dependencies: ncurses_sh,
)