project('sfmlapp', 'cpp',
    default_options: ['cpp_std=c++17',
                      'wrap_mode=forcefallback',
		      'default_library=static',
		      'buildtype=debugoptimized',
                     ])

cpp = meson.get_compiler('cpp')

sfml_dep = dependency('sfml')
imgui_sfml_dep = dependency('imgui-sfml')

executable('sfml-test', 'sfmltest.cpp',
    win_subsystem: 'windows',
    dependencies: [imgui_sfml_dep, sfml_dep])
