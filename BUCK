cxx_library(
  name = 'mujs',
  header_namespace = '',
  exported_headers = [
    'mujs.h',
  ],
  headers = subdir_glob([
    ('', '*.h'),
    ('', '*.c'),
  ], excludes = [
    'mujs.h',
    'one.c',
  ]),
  srcs = glob([
    'one.c',
  ]),
  visibility = [
    'PUBLIC',
  ],
)

cxx_binary(
  name = 'mujs-cli',
  srcs = [
    'main.c',
  ],
  deps = [
    ':mujs',
  ],
)
