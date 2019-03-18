project('zlib-ng', 'c', version : '0.1', license : 'zlib')

zlibng_inc = include_directories('.')

cdata = configuration_data()

configure_file(
    input : 'zconf-ng.h.meson',
    output : 'zconf-ng.h',
    configuration : cdata)

zlibng_src = files([
    'adler32.c',
    'compress.c',
    'crc32.c',
    'crc32.h',
    'deflate.c',
    'deflate_fast.c',
    'deflate_medium.c',
    'deflate_slow.c',
    'functable.c',
    'gzclose.c',
    'gzlib.c',
    'gzread.c',
    'gzwrite.c',
    'infback.c',
    'inffast.c',
    'inflate.c',
    'inftrees.c',
    'trees.c',
    'uncompr.c',
    'zutil.c'
])

subdir('arch')

zlibng_lib = library('zlib-ng', zlibng_src)

zlibng_dep = declare_dependency(link_with : zlibng_lib,
                                 include_directories : zlibng_inc)
                            
