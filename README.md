# libpdfium

pdfium build based on a GNU Makefile

# Getting the source

git clone --recurse-submodules https://github.com/vtorri/libpdfium.git

# Setting build system

cd libpdfium/pdfium
mkdir build && cd build
cp ../../build_config.h ../../Makefile_pdfium .
