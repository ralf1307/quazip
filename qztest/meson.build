qt = import('qt5')
src = []
deps = []

qt_modules = ['Core', 'Network', 'Test']
qt_dep = dependency('qt5', modules: qt_modules)
deps += qt_dep

moc_src = [
'qztest.cpp',
'testjlcompress.cpp',
'testquachecksum32.cpp',
'testquagzipfile.cpp',
'testquaziodevice.cpp',
'testquazip.cpp',
'testquazipdir.cpp',
'testquazipfile.cpp',
'testquazipfileinfo.cpp',
'testquazipnewinfo.cpp',
]

moc_srch = [
'qztest.h',
'testjlcompress.h',
'testquachecksum32.h',
'testquagzipfile.h',
'testquaziodevice.h',
'testquazip.h',
'testquazipdir.h',
'testquazipfile.h',
'testquazipfileinfo.h',
'testquazipnewinfo.h',
]

src += qt.compile_moc(
sources: moc_src,
headers: moc_srch,
dependencies: qt_dep,
)


qztest_exe = executable('qztest', src, dependencies: deps, link_with: quazip_lib)
test('qztest', qztest_exe)
