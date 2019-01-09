project('buildyourownlisp', 
	'c',        
	version: '0.1.0',
  	meson_version: '>= 0.40.0',)

c_compiler = meson.get_compiler('c')
readline_dep = c_compiler.find_library('readline', required: false)

config_h = configuration_data()
config_h.set_quoted('PACKAGE_VERSION', meson.project_version())
configure_file(
  output: 'buildyourownlisp-config.h',
  configuration: config_h,
)
add_project_arguments([
  '-I' + meson.build_root(),
], language: 'c')

subdir('src')
