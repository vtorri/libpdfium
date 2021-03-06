# libpdfium

pdfium build based on a GNU Makefile

# Getting the source

git clone --recurse-submodules https://github.com/vtorri/libpdfium.git

# Setting build system

* cd libpdfium/pdfium
* git checkout chromium/3940
* mkdir build
* cp ../build_config.h build
* cp ../Makefile.pdfium .
* cp ../libpkgconfig.pc.in .

In addition, on Windows:

* cp ../patch.diff .
* patch -p1 < patch.diff

# Compilation and installation

* make -f Makefile_pdfium OS=my_os
* make -f Makefile_pdfium install

 you can of course run 'make' in parallal mode

# Aditional rules

* 'make -f Makefile_pdfium help' for the help
* 'make -f Makefile_pdfium status' to know where the files will be installed, the arch, etc...

# Example of compilation on Windows:

* make -j 8 -f Makefile.pdfium prefix=/opt/pdfium OS=Windows install
