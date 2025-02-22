project('vulkanEngine', 'c',
        default_options: 'default_library=static')

subdir('src')
subdir('src/vulkan')

src = [mainSrc, vulkanSrc]

vulkanDep = dependency('vulkan')
sdl3Dep = dependency('sdl3')

incdir = include_directories('include', '/opt/homebrew/include')

executable('vulkanEngine', src,
           dependencies: [sdl3Dep, vulkanDep],
           include_directories: incdir)
