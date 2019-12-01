project('tllist', 'c', version: '1.0.0', license: 'MIT', meson_version: '>=0.50.0')
tllist = declare_dependency(include_directories: '.')

unittest = executable('unittest', 'test.c', dependencies: [tllist])
test('unittest', unittest)

if not meson.is_subproject()
  install_headers('tllist.h')

  pkg = import('pkgconfig')
  pkg.generate(libraries : [],
               subdirs : ['.'],
               name : 'tllist',
               filebase : 'tllist',
               description : 'A C header file only implementation of a typed linked list')
endif
