zlibng_src += files('x86.c')

add_project_arguments('-msse2', language : 'c')
zlibng_src += files('fill_window_sse.c')

add_project_arguments('-msse4', language : 'c')
add_project_arguments('-mpclmul', language : 'c')

zlibng_src += files('insert_string_sse.c')

