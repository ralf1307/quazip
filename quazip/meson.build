src = [
'crypt.h',
'ioapi.h',
'JlCompress.cpp',
'JlCompress.h',
'qioapi.cpp',
'quaadler32.cpp',
'quaadler32.h',
'quachecksum32.h',
'quacrc32.cpp',
'quacrc32.h',
'quagzipfile.cpp',
'quagzipfile.h',
'quaziodevice.cpp',
'quaziodevice.h',
'quazip.cpp',
'quazip.h',
'quazip_global.h',
'quazipdir.cpp',
'quazipdir.h',
'quazipfile.cpp',
'quazipfile.h',
'quazipfileinfo.cpp',
'quazipfileinfo.h',
'quazipnewinfo.cpp',
'quazipnewinfo.h',
'unzip.c',
'unzip.h',
'zip.c',
'zip.h',
]

dep = []

qt = import('qt5')
qt_modules = ['Core']
dep += dependency('qt5', modules: qt_modules)
dep += dependency('zlib')

quazip_lib = library('quazip', dependencies: dep)
quazip_dep = declare_dependency(
  link_with: quazip_lib,
)
