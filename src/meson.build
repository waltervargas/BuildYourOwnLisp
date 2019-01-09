buildyourownlisp_sources = [
  'parsing.c',
  'mpc.c',
]

buildyourownlisp_deps = [
  dependency('glib-2.0'),
]

executable('buildyourownlisp', buildyourownlisp_sources,
  dependencies: [ buildyourownlisp_deps, readline_dep],
  install: true,
)
