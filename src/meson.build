testsubmission_sources = [
  'main.vala',
  'application.vala',
  'window.vala',
]

testsubmission_deps = [
  config_dep,
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.4'),
]

testsubmission_sources += gnome.compile_resources('testsubmission-resources',
  'testsubmission.gresource.xml',
  c_name: 'testsubmission'
)

executable('testsubmission', testsubmission_sources,
  dependencies: testsubmission_deps,
  include_directories: config_inc,
       install: true,
)
